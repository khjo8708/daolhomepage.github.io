<script setup>
defineProps({
  variant: {
    type: String,
    default: "gradient",
  },
  color: {
    type: String,
    default: "success",
  },
  size: {
    type: String,
    default: "md",
  },
  icon: {
    type: [String, Object],
    required: true,
    component: String,
    color: String,
  },
  iconNumber :{
    type: [String, Number], // 변경: 아이콘 번호를 문자열 또는 숫자로 설정
    default: ""

  },
  content: {
    type: String,
    required: true,
  },
});

function backgroundColor(variant, color) {
  let colorValue;

  if (variant === "gradient") {
    colorValue = "bg-gradient-" + color;
  } else if (variant === "contained") {
    colorValue = "bg-" + color;
  }

  return colorValue;
}
</script>


<template>
  <div class="p-3 d-flex align-content-center">
    <div
      class="icon icon-shape text-center border-radius-xl"
      :class="`icon-${size} ${backgroundColor(variant, color)} shadow-${color}`"
    >
      <span class="icon-number">{{ iconNumber }}</span>
    </div>
    <div class="description ps-3">
      <p class="mb-0" v-html="content" />
    </div>
  </div>
</template>


<style scoped>

.description {
  width: 100%;
}

p {
  font-size: 20px; /* 콘텐츠의 기본 폰트 크기 설정 */
}

.icon {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 30px; /* Adjust size if needed */
  height: 50px; /* Adjust size if needed */
  width: 80px; /* Adjust size if needed */
  position: relative;
}

.icon-number {
  bottom: 5px; /* Adjust positioning */
  right: 5px; /* Adjust positioning */
  font-size: 20px; /* Adjust text size */
  color: white; /* Adjust text color */
}
/* 기타 필요한 스타일 추가 */


</style>

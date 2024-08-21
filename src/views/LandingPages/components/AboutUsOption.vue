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

.container{

  display: flex;
}

/* 기타 필요한 스타일 추가 */


</style>

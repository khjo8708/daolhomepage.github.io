<script setup>

defineProps({
  breadcrumb: {
    type: Array,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
});
</script>
<template>

  <div class="container mt-5">
    <div class="row">
      <div class="col-lg-12 mx-auto text-center ">
        <div class="full-width align-self-center  custom-margin">
          <h1>{{ title }}</h1>
        </div>

        <slot />
      </div>
    </div>
  </div>
  <CenteredFooter />
</template>


<style scoped>
.custom-margin {
  margin-bottom: 30px;
}
</style>

<script setup>
import ExampleCard from "../Components/ExampleCard.vue";
import MaterialBadge from "../../../components/MaterialBadge.vue";

// image
import DoppBusi from "@/assets/img/dopp-busi.png";
</script>
<template>
  <section class="my-5 py-5">
    <div class="container">
      <div class="row">
        <div class="row justify-content-center text-center my-sm-5">
          <div class="col-lg-6">
            <MaterialBadge color="success" class="mb-3"
              size="300">Infinite combinations</MaterialBadge
            >
            <h2 class="text-dark mb-0">사업 분야</h2>
          </div>
          <p class="lead row justify-content-center">
            <img :src="`${DoppBusi}`"  alt=""/>
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

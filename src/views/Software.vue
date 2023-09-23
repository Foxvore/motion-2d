<script setup>
import { onMounted } from "vue";
import HalfHeader from "@/components/HalfHeader.vue";
import SoftwareLibrary from "@/components/software/SoftwareLibrary.vue";

onMounted(() => {
  window.scrollTo(0, 0);
});
</script>

<template>
  <section id="header">
    <HalfHeader title="Software" subtitle="for Making Motion 2D" />
  </section>

  <section id="software-library" class="px-[120px] py-[50px] h-auto">
    <SoftwareLibrary />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>
</template>

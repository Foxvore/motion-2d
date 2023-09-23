<script setup>
import HalfHeader from "@/components/HalfHeader.vue";
import Transisi from "@/components/motion-2d/Transisi.vue";
</script>

<template>
  <section id="header">
    <HalfHeader title="What is Motion 2D?" subtitle="Definition & Function" />
  </section>

  <section id="transition" class="px-[120px] my-[50px] h-auto">
    <Transisi />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>
</template>

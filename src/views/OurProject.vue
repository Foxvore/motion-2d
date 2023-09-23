<script setup>
import { onMounted } from "vue";
import HalfHeader from "@/components/HalfHeader.vue";
import OurTeam from "@/components/our-project/OurTeam.vue";
import Motion from "@/components/our-project/Motion.vue";

onMounted(() => {
  window.scrollTo(0, 0);
});
</script>

<template>
  <section id="header">
    <HalfHeader title="Our Project" subtitle="and Tri'sta Members" />
  </section>

  <section id="our-team" class="px-[120px] h-auto">
    <OurTeam />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>

  <section id="our-team" class="px-[120px] my-[50px] h-auto">
    <Motion />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>
</template>

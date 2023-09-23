<script setup>
import { onMounted } from "vue";
import Header from "@/components/Header.vue";
import Definition from "@/components/homepage/Definition.vue";
import Software from "@/components/homepage/Software.vue";
import Tutorial from "@/components/homepage/Tutorial.vue";
import OurProject from "@/components/homepage/OurProject.vue";

onMounted(() => {
  window.scrollTo(0, 0);
});
</script>

<template>
  <section id="carousel">
    <Header />
  </section>

  <section id="definition" class="py-[50px] px-[120px] h-auto">
    <Definition />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>

  <section id="software" class="py-[50px] px-[120px] h-auto">
    <Software />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>

  <section id="tutorial" class="py-[50px] px-[120px] h-auto">
    <Tutorial />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>

  <section id="tutorial" class="py-[50px] px-[120px] h-auto">
    <OurProject />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>
</template>

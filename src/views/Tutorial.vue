<script setup>
import { onMounted } from "vue";
import HalfHeader from "@/components/HalfHeader.vue";
import LinkLibrary from "@/components/tutorial/LinkLibrary.vue";

onMounted(() => {
  window.scrollTo(0, 0);
});
</script>

<template>
  <section id="header">
    <HalfHeader title="Tutorial" subtitle="for Making Motion 2D" />
  </section>

  <section id="our-team" class="px-[120px] py-[50px] h-auto">
    <LinkLibrary />
  </section>

  <div class="px-[70px]">
    <hr />
  </div>
</template>

<script setup></script>

<template>
  <div class="img-background">
    <div
      class="carousel absolute flex h-screen w-full items-center justify-center z-40"
    >
      <div>
        <p
          class="text-9xl text-white text-center font-bold drop-shadow-lg tracking-widest"
        >
          MOTION 2D
        </p>
        <p
          class="text-3xl text-white text-center font-bold drop-shadow-lg tracking-wider"
        >
          by Tri'sta
        </p>
      </div>
    </div>
    <div class="absolute h-screen w-full bg-black opacity-50 z-10" />
  </div>
</template>

<style scoped>
.img-background {
  width: 100%;
  height: 100vh;
  background: url("@/assets/img/thumbnail.png") top center;
  background-attachment: fixed;
  background-size: cover;
  position: relative;
  box-shadow: 2px 0 35px 0 rgba(68, 88, 144, 0.5);
}

.carousel {
  font-family: "Bebas Neue", sans-serif !important;
}
</style>

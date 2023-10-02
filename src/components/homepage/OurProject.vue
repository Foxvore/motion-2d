<script setup></script>

<template>
  <div class="grid grid-cols-2">
    <div class="flex items-center">
      <div class="flex justify-start items-center pr-32">
        <div class="card" style="--rating: 90">
          <img
            src="@/assets/img/project/vid_thumbnail.png"
            alt=""
            class="w-full rounded-lg"
          />
        </div>
      </div>
    </div>
    <div class="flex items-center">
      <div>
        <p class="title text-4xl mb-5">Our Project</p>
        <p class="mb-3 text-justify">
          <b>"What is Motion 2D?"</b> merupakan sebuah video Motion 2D karya
          kelompok 3 yaitu
          <b class="text-[var(--primary-color)]">Tri'sta.</b> Video ini berisi
          tentang penjelasan, fungsi, dan contoh penggunaan dari Motion 2D.
        </p>
        <router-link :to="{ name: 'Our Project' }">
          <button class="learn-more mt-5 !w-[14rem]">
            <span class="circle" aria-hidden="true">
              <span class="icon arrow"></span>
            </span>
            <span class="button-text">Tonton video</span>
          </button>
        </router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  width: auto;
  height: auto;
  background: var(--quaternary-color);
  border: 1px solid var(--cardBorder);
  padding: 7px;
  box-shadow: 8px 8px 0 var(--secondary-color);
  transition: box-shadow 0.5s, transform 0.5s;
  border-radius: 8px;
  display: inline-block;
}

.card:hover {
  transform: translate(-2px, -4px);
  box-shadow: 16px 16px 0 var(--tertiary-color);
}
</style>

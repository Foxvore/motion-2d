<script setup></script>

<template>
  <div class="grid grid-cols-3">
    <div class="col-span-2 flex items-center">
      <div>
        <p class="title text-4xl mb-5">Tutorial</p>
        <p class="mb-3 text-justify">
          Webiste memuat link video tutorial yang yang dapat kalian ikuti untuk
          membuat video motion 2D dengan menggunakan software
          <b>Adobe After Effect</b> dan <b>Adobe Animate</b>.
        </p>
        <p class="mb-3 text-justify">
          Terdapat 6 link yang dapat diakses untuk menonton video tutorial
          membuat Motion 2D mengunakan <b>Adobe After Effect</b> dan 10 link
          yang dapat diakses untuk menonton video tutorial membuat Motion 2D
          mengunakan <b>Adobe Animate</b>.
        </p>
        <router-link :to="{ name: 'Tutorial' }">
          <button class="learn-more mt-5 !w-[17rem]">
            <span class="circle" aria-hidden="true">
              <span class="icon arrow"></span>
            </span>
            <span class="button-text">Lihat selengkapnya</span>
          </button>
        </router-link>
      </div>
    </div>
    <div class="flex justify-center items-center">
      <img
        src="@/assets/gif/homepage/tutorial.gif"
        alt="def.giv"
        class="w-[300px] h-[300px]"
      />
    </div>
  </div>
</template>

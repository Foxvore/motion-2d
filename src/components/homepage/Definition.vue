<script setup></script>

<template>
  <div class="grid grid-cols-3">
    <div class="col-span-2 flex items-center">
      <div>
        <p class="title text-4xl mb-5">What is Motion 2D?</p>
        <p class="mb-3 text-justify">
          Motion 2D merupakan cabang ilmu desain grafis yang dapat menggabungkan
          teks, warna, grafik, dan gerakan untuk memberikan kehidupan dan
          merekam mereka menjadi sebuah pesan yang ingin di sampaikan kepada
          penontonnya.
        </p>
        <p class="mb-3 text-justify">
          Motion 2D mengacu pada pergerakan objek atau elemen dalam dua dimensi.
          Ini melibatkan penggunaan animasi untuk menciptakan ilusi pergerakan
          dan dinamika. Motion 2D digunakan dalam iklan, animasi karakter dalam
          permainan, dan efek visual dalam film atau video dan maish banyak
          lagi.
        </p>
        <router-link :to="{ name: 'Motion 2D' }">
          <button class="learn-more mt-5 !w-[21rem]">
            <span class="circle" aria-hidden="true">
              <span class="icon arrow"></span>
            </span>
            <span class="button-text">Baca materi selengkapnya</span>
          </button>
        </router-link>
      </div>
    </div>
    <div class="flex justify-center items-center">
      <img
        src="@/assets/giv/homepage/definition.gif"
        alt="def.giv"
        class="w-[300px] h-[300px]"
      />
    </div>
  </div>
</template>

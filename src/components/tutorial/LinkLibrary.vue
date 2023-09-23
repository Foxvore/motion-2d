<script setup>
const tutorial = [
  {
    title: "Ternyata Desain Ada Prinsipnya!",
    channel: "Kok Bisa?",
    link: "https://www.youtube.com/embed/lWAWSvVp5pI?si=YUgdHH3AHlqI9In6",
    date: "28 Oktober 2022",
    desc: "Belajar prinsip sebuah design",
  },
  {
    title: "Ternyata Desain Ada Prinsipnya!",
    channel: "Kok Bisa?",
    link: "https://www.youtube.com/embed/lWAWSvVp5pI?si=YUgdHH3AHlqI9In6",
    date: "28 Oktober 2022",
    desc: "Belajar prinsip sebuah design",
  },
  {
    title: "Ternyata Desain Ada Prinsipnya!",
    channel: "Kok Bisa?",
    link: "https://www.youtube.com/embed/lWAWSvVp5pI?si=YUgdHH3AHlqI9In6",
    date: "28 Oktober 2022",
    desc: "Belajar prinsip sebuah",
  },
  {
    title: "Ternyata Desain Ada Prinsipnya!",
    channel: "Kok Bisa?",
    link: "https://www.youtube.com/embed/lWAWSvVp5pI?si=YUgdHH3AHlqI9In6",
    date: "28 Oktober 2022",
    desc: "Belajar prinsip sebuah design",
  },
];
</script>

<template>
  <!-- <div class="text-center mb-5 font-bold">
    Dibawah ini ada cideo tutorial yang dapat digunakan untuk membuat motion 2D,
    mulai dari pembuatan assets sampai memberinkan motion pada assets 2D
  </div>

  <hr class="my-5" /> -->

  <div class="grid grid-flow-row grid-cols-3">
    <el-card v-for="item in tutorial" :key="item" class="card mx-2 my-2">
      <div class="flex justify-center">
        <iframe
          class="rounded-md"
          width="447"
          height="245"
          :src="item.link"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
        ></iframe>
      </div>
      <div class="mt-4">
        <div class="mb-1">
          <p class="text-gray-400 text-xs">Title</p>
          <p class="font-bold text-base">
            {{ item.title }}
          </p>
        </div>
        <div class="mb-1">
          <p class="text-gray-400 text-xs">Channel</p>
          <p class="font-bold text-base">
            {{ item.channel }}
          </p>
        </div>
        <div class="mb-1">
          <p class="text-gray-400 text-xs">Upload Date</p>
          <p class="font-bold text-base">
            {{ item.date }}
          </p>
        </div>
        <div>
          <p class="text-gray-400 text-xs">Description</p>
          <p class="font-bold text-base">
            {{ item.desc }}
          </p>
        </div>
      </div>
    </el-card>
  </div>

  <!-- <hr class="my-3" />

  <div class="grid grid-flow-row grid-cols-2">
    <el-card v-for="item in tutorial" :key="item" class="card m-2">
      <div class="grid grid-cols-3">
        <div>
          <div class="bg-white w-full h-auto">
            <iframe
              class="rounded-md"
              width="227"
              height="128"
              :src="item.link"
              title="YouTube video player"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
          </div>
        </div>
        <div class="col-span-2 px-3 flex items-center">
          <div>
            <div class="mb-1">
              <p class="text-gray-400 text-xs">Title</p>
              <p class="font-bold text-base">
                {{ item.title }}
              </p>
            </div>
            <div class="mb-1">
              <p class="text-gray-400 text-xs">Channel</p>
              <p class="font-bold text-base">
                {{ item.channel }}
              </p>
            </div>
            <div>
              <p class="text-gray-400 text-xs">Upload Date</p>
              <p class="font-bold text-base">
                {{ item.date }}
              </p>
            </div>
          </div>
        </div>
        <div class="mt-4">
          <p class="text-gray-400 text-xs">Description</p>
          <p class="font-bold text-base">
            {{ item.desc }}
          </p>
        </div>
      </div>
    </el-card>
  </div> -->
</template>

<style scoped>
.card:hover {
  scale: 1.02;
}
</style>

<script setup>
const tutorial_an = [
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
    desc: "Belajar prinsip sebuah design",
  },
];
</script>

<template>
  <div class="title text-4xl text-center mb-5">
    Adobe After Effect tutorial by TipTut (ENG)
  </div>

  <div class="overflow-auto whitespace-nowrap">
    <el-card
      v-for="item in tutorial_an"
      :key="item"
      class="card mx-2 my-2 inline-block"
    >
      <div class="flex justify-center">
        <iframe
          class="rounded-md"
          width="280"
          height="157"
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
</template>

<style scoped>
.card:hover {
  scale: 1.02;
}

::-webkit-scrollbar {
  height: 5px !important;
}

::-webkit-scrollbar-thumb {
  background-image: linear-gradient(
    to right,
    var(--primary-color),
    var(--secondary-color),
    var(--tertiary-color),
    var(--quaternary-color)
  );
  border-radius: 10px;
}
</style>

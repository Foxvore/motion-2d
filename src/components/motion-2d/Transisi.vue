<script setup>
const transisi = [
  {
    example: "",
    name: "Cut",
    desc: "Ini adalah jenis transisi yang paling sederhana. Saat satu adegan atau gambar tiba-tiba digantikan oleh adegan atau gambar berikutnya tanpa efek khusus.",
  },
  {
    example: "",
    name: "Fade",
    desc: "Aset yang satu muncul perlahan-lahan sementara aset lainnya menghilang perlahan-lahan. Ini menciptakan efek transisi yang lembut.",
  },
  {
    example: "",
    name: "Slide",
    desc: "Dalam gerakan slide, aset bergerak secara horizontal atau vertikal untuk memberikan perpindahan antara elemen yang satu dengan yang lainnya.",
  },
  {
    example: "",
    name: "Zoom",
    desc: "Pada gerakan zoom, kamera atau pandangan pemirsa bergerak mendekat atau menjauh dari objek, menciptakan efek perubahan skala.",
  },
  {
    example: "",
    name: "Rotate",
    desc: ": Aset dapat berputar untuk mengubah transisi dari satu elemen ke elemen lainnya. Ini sering digunakan untuk memberikan efek perubahan sudut pandang.",
  },
  {
    example: "",
    name: "Flip",
    desc: "Dalam gerakan flip, aset dapat diputar secara horizontal atau vertikal untuk menciptakan efek cermin atau pembalikan.",
  },
  {
    example: "",
    name: "Dissolve",
    desc: "Pada transisi dissolve, aset yang satu mulai memudar secara perlahan-lahan sementara aset yang lain muncul. Ini menciptakan efek transisi yang lembut.",
  },
  {
    example: "",
    name: "Masking",
    desc: "Dalam masking, elemen tertentu digunakan sebagai masker untuk mengungkap elemen di belakangnya secara perlahan-lahan. Ini sering digunakan untuk mengubah bentuk elemen.",
  },
  {
    example: "",
    name: "Particle Effects",
    desc: "Gerakan transisi dapat melibatkan efek partikel seperti percikan, debu, atau bintang yang muncul atau menghilang untuk menghubungkan dua elemen.",
  },
];
</script>

<template>
  <p class="title text-4xl mb-5 text-center">
    Jenis-jenis Transformasi Transisi
  </p>

  <div class="grid grid-flow-row grid-cols-3">
    <el-card v-for="item in transisi" :key="item" class="transition-card m-2">
      <div
        class="w-full h-[250px] bg-gray-400 rounded-md mb-3 flex justify-center items-center"
      >
        Contoh Transisi
      </div>
      <p class="title text-2xl text-center">{{ item.name }}</p>
      <p class="text-justify p-3">{{ item.desc }}</p>
    </el-card>
  </div>
</template>

<style scoped>
.transition-card:hover {
  scale: 1.02;
}
</style>

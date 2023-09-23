<script setup>
import Illustrator from "@/assets/img/software-requirement/ai.png";
import AfterEffect from "@/assets/img/software-requirement/ae.png";
import Animiate from "@/assets/img/software-requirement/an.png";

const software = [
  // {
  //   logo: Illustrator,
  //   name: "Adobe Illustration",
  //   inc: "Adobe Inc.",
  //   function: "Untuk membuat assets 2D",
  //   link: "https://www.adobe.com/id_en/products/illustrator.html",
  //   cpu: "Multicore Intel processor (with 64-bit support) with SSE 4.2 or later or AMD Athlon 64 processor with SSE 4.2 or later.",
  //   os: "Windows 11 and Windows 10 (64-bit) versions V21H1, and V20H2. Windows Server versions V1607 (2016) and V1809 (2019).",
  //   ram: "8 GB of RAM (16 GB recommended).",
  //   hdd: "2 GB of available hard-disk space for installation. Additional free space required during installation. (SSD recommended)",
  //   monitor:
  //     "1024 x 768 display (1920 x 1080 recommended). To use Touch workspace in Illustrator, you must have a touch-screen-enabled tablet/monitor running Windows 10 (Microsoft Surface Pro 3 recommended).",
  //   gpu: "Have a minimum of 1 GB of VRAM (4 GB recommended). Support OpenGL version 4.0 or greater.",
  //   internet:
  //     "Internet connection and registration are necessary for required software activation, validation of subscriptions, and access toonline services.",
  // },
  {
    logo: AfterEffect,
    name: "Adobe After Effect",
    inc: "Adobe Inc.",
    function: "Untuk memberikan gerakan kepada aset 2D",
    link: "https://www.adobe.com/id_en/products/aftereffects.html",
    cpu: "Intel or AMD Quad-Core Processor (8-Core or above for Multi-Frame Rendering recommended).",
    os: "Microsoft Windows 10 (64-bit) V20H2 or later.",
    ram: "16 GB of RAM (32 GB recommended).",
    hdd: "15GB of available hard-disk space; additional free space required during installation (cannot install on removable flash storage devices). Additional disk space for disk cache (64GB+ recommended).",
    monitor: "1920 x 1080 (1920x1080 or greater display resolution).",
    gpu: "2 GB of GPU VRAM (4GB or more of GPU VRAM recommended). Note: For systems with NVIDIA GPUs, Windows 11 requires NVIDIA driver version 472.12 or later.",
    internet:
      "Internet connection and registration are necessary for required software activation, validation of subscriptions, and access toonline services.",
  },
  {
    logo: Animiate,
    name: "Adobe Animate",
    inc: "Adobe Inc.",
    function: "Untuk memberikan gerakan kepada aset 2D",
    link: "https://www.adobe.com/id_en/products/animate.html",
    cpu: "Intel Pentium 4 or Intel Centrino, Intel Xeon, or Intel Core Duo (or compatible) processor (2GHz or faster processor).",
    os: "Windows 10 version V20H2, V21H1.",
    ram: "8 GB of RAM (16 GB recommended).",
    hdd: "4 GB of available hard-disk space for installation; more free space required during installation (cannot install on removable flash storage devices).",
    monitor: "1024x900 display (1280x1024 recommended).",
    gpu: "OpenGL version 3.3 or higher (DirectX 12 with feature level 12_0 recommended).",
    internet:
      "Internet connection and registration are necessary for required software activation, validation of subscriptions, and access to online services.",
  },
];

const openWeb = (link) => {
  window.open(link);
};
</script>

<template>
  <div class="grid grid-flow-row grid-cols-2">
    <el-card v-for="item in software" :key="item" class="el-card h-full m-3">
      <div class="flex justify-center">
        <div>
          <div class="mb-5 text-center">
            <p class="title text-3xl">{{ item.name }}</p>
            <p class="text-gray-400 text-sm">{{ item.inc }}</p>
          </div>
          <div class="mb-5 flex justify-center">
            <img :src="item.logo" alt="Adobe Illustrator" class="w-[300px]" />
          </div>
          <div class="mb-5 text-center">
            <p class="text-gray-500 text-sm mb-1">
              Kegunaan : {{ item.function }}
            </p>
            <p class="link text-gray-500 text-xs" @click="openWeb(item.link)">
              <b>Klik disini untuk mengunjungi website {{ item.name }}</b>
            </p>
          </div>
        </div>
      </div>
      <hr class="mb-5" />
      <div class="mx-5">
        <div class="mb-3">
          <p class="title text-xl">Processor</p>
          <p class="text-gray-500 text-sm">
            {{ item.cpu }}
          </p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">Operating System</p>
          <p class="text-gray-500 text-sm">
            {{ item.os }}
          </p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">RAM</p>
          <p class="text-gray-500 text-sm">{{ item.ram }}</p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">Hard Disk</p>
          <p class="text-gray-500 text-sm">
            {{ item.hdd }}
          </p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">Monitor Resolution</p>
          <p class="text-gray-500 text-sm">
            {{ item.monitor }}
          </p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">GPU</p>
          <p class="text-gray-500 text-sm">
            {{ item.gpu }}
          </p>
        </div>
        <div class="mb-3">
          <p class="title text-xl">Internet Connection</p>
          <p class="text-gray-500 text-sm">
            {{ item.internet }}
          </p>
        </div>
      </div>
    </el-card>
  </div>
</template>

<style scoped>
.el-card:hover {
  scale: 1.03;
}

.link {
  cursor: pointer;
}

.link:hover {
  color: var(--secondary-color);
}
</style>

<script setup>
import { onMounted } from "vue";

onMounted(() => {
  scroll();
});

const scroll = () => {
  document.addEventListener("scroll", () => {
    const navbar = document.querySelector(".navbar");
    if (window.scrollY > 100) {
      navbar.classList.add("navbar-scrolled");
    } else {
      navbar.classList.remove("navbar-scrolled");
    }

    const top = document.querySelector(".back-to-top");
    if (window.scrollY > 100) {
      top.classList.add("active");
    } else {
      top.classList.remove("active");
    }
  });
};
</script>

<template>
  <nav
    class="navbar absolute px-[50px] py-[20px] flex justify-between items-center w-full box-border z-50 text-white"
  >
    <a href="#" class="font-bold text-[2.5rem] tracking-wider">Tri'sta</a>
    <div>
      <ul class="flex text-[1.1rem]">
        <li class="mx-[20px]">
          <button class="btn-router">
            <router-link :to="{ name: 'Homepage' }" class="tracking-wide">
              Homepage
            </router-link>
          </button>
        </li>
        <li class="mx-[20px]">
          <button class="btn-router">
            <router-link :to="{ name: 'Motion 2D' }" class="tracking-wide">
              What is Motion 2D?
            </router-link>
          </button>
        </li>
        <li class="mx-[20px]">
          <button class="btn-router">
            <router-link :to="{ name: 'Software' }" class="tracking-wide">
              Software
            </router-link>
          </button>
        </li>
        <li class="mx-[20px]">
          <button class="btn-router">
            <router-link :to="{ name: 'Tutorial' }" class="tracking-wide">
              Tutorial
            </router-link>
          </button>
        </li>
        <li class="mx-[20px]">
          <button class="btn-router">
            <router-link :to="{ name: 'Our Project' }" class="tracking-wide">
              Our Project
            </router-link>
          </button>
        </li>
      </ul>
    </div>
  </nav>

  <div id="back-to-top" class="back-to-top">
    <a href="#" class="text-[var(--quaternary-color)] font-bold text-3xl">
      <i class="fa-solid fa-circle-chevron-up"></i>
    </a>
  </div>
</template>

<style scoped>
.navbar {
  font-family: "Bebas Neue", sans-serif !important;
  position: fixed;
  transition: var(--tran-05);
}

.navbar.navbar-scrolled {
  background: rgba(27, 26, 23, 0.7);
  padding: 15px 50px;
  backdrop-filter: blur(5px);
}

.btn-router {
  position: relative;
  cursor: pointer !important;
  transition-timing-function: cubic-bezier(0.25, 0.8, 0.25, 1);
  transition-duration: 400ms;
  transition-property: color;
}

.btn-router li {
  cursor: pointer;
}

a.active,
.btn-router:hover {
  color: var(--tertiary-color);
}

a.active:after,
.btn-router:hover:after {
  width: 100%;
  left: 0%;
}

a:after,
.btn-router:after {
  content: "";
  pointer-events: none;
  bottom: -2px;
  left: 50%;
  position: absolute;
  width: 0%;
  height: 2px;
  background-color: var(--primary-color);
  transition-timing-function: cubic-bezier(0.25, 0.8, 0.25, 1);
  transition-duration: 400ms;
  transition-property: width, left;
}

.back-to-top {
  visibility: hidden;
  opacity: 0;
  position: fixed;
  right: 15px;
  bottom: 15px;
  z-index: 100;
  background: var(--primary-color);
  width: 40px;
  height: 40px;
  border-radius: 50px;
  transition: var(--tran-03);
  display: flex;
  align-items: center;
  justify-content: center;
}

.back-to-top:hover {
  background: var(--secondary-color);
  scale: 1.1;
}

.back-to-top.active {
  visibility: visible;
  opacity: 1;
}
</style>

<script setup></script>

<template>
  <p class="title text-4xl mb-5 text-center">Our Project</p>
  <div class="flex justify-center">
    <div class="card">
      <div class="card-image">
        <iframe
          class="rounded-md"
          width="800"
          height="450"
          src="https://www.youtube.com/embed/U2anTtDa03c?si=aIy4fk2E4lb0wB60"
          title="What is Motion 2D? - Tri'sta Project"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          allowfullscreen
        />
      </div>
      <div class="category">
        <button class="button">Motion 2D Video</button>
      </div>
      <div class="heading">
        What is Motion 2D?
        <div class="author">
          By <span class="name">Tri'sta</span> - 30 Desember 2023
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  width: auto;
  height: 100%;
  background: var(--secondary-color);
  padding: 0.4em;
  border-radius: 6px;
  border: 2px solid black;
}

.card-image {
  background-color: rgb(236, 236, 236);
  width: 100%;
  height: 100%;
  border-radius: 6px;
}

.category {
  text-transform: uppercase;
  color: white;
  padding: 10px 3px 6px 7px;
}

.category .button {
  background: white;
  color: var(--primary-color);
  font-size: 0.8em;
  font-weight: 800;
  border: none;
  border-radius: 6px;
  padding: 0.4rem 0.6rem;
  box-shadow: rgba(165, 132, 130, 0.1333333333) 0px 5px 5px 0px;
  transition: var(--tran-03);
}

.category .button:hover {
  background: var(--primary-color);
  color: white;
}

.heading {
  font-weight: 600;
  font-size: 1.5em;
  color: white;
  padding: 0 7px;
}

.author {
  color: white;
  font-weight: 400;
  font-size: 11px;
  padding-top: 10px;
  padding-bottom: 3px;
}

.name {
  font-weight: 600;
}

.name:hover {
  cursor: pointer;
}
</style>

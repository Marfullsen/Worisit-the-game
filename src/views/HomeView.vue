<template>
  <div class="gradiente">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <h1 class="text-7xl neonText">Worisit</h1>
    <blockquote
      class="mt-4 text-2xl font-semibold italic text-center text-white"
    >
      ¡Adivina
      <span
        class="before:block before:absolute before:-inset-1 before:-skew-y-3 before:bg-pink-500 relative inline-block"
      >
        <span class="relative text-white">qué fue</span>
      </span>
      lo que escribieron!
    </blockquote>
    <div class="mt-12 mb-3 pt-0 flex justify-center">
      <input
        type="text"
        placeholder="Fulanito Perez"
        class="w-60 text-center px-3 py-3 placeholder-slate-300 text-slate-600 bg-white bg-white rounded-full text-sm border-0 shadow outline-none focus:outline-none focus:ring w-full"
      />
    </div>
    <button
      class="px-3 py-2 rounded-full bg-gradient-to-r from-violet-600 to-fuchsia-600"
    >
      ¡Jugar!
    </button>

    <!-- Toggle A -->
    <div class="flex items-center justify-center w-full mb-12">
      <div class="ml-3 font-medium">Todos contra todos&nbsp;&nbsp;&nbsp;</div>
      <label for="toogleA" class="flex items-center cursor-pointer">
        <!-- toggle -->
        <div class="relative">
          <!-- input -->
          <input id="toogleA" type="checkbox" class="sr-only" />
          <!-- line -->
          <div class="w-10 h-4 bg-gray-400 rounded-full shadow-inner"></div>
          <!-- dot -->
          <div
            class="dot absolute w-6 h-6 bg-white rounded-full shadow -left-1 -top-1 transition"
          ></div>
        </div>
        <!-- label -->
        <div class="ml-3 font-medium">Equipos</div>
      </label>
    </div>

    <div class="mt-12 mb-3 pt-0 flex justify-center">
      <button
        class="w-15 px-3 py-2 rounded-full bg-gradient-to-r from-violet-600 to-fuchsia-600"
      >
        Crear
      </button>
      <button
        class="w-15 px-3 py-2 rounded-full bg-gradient-to-r from-violet-600 to-fuchsia-600"
      >
        Unirse
      </button>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
/* import HelloWorld from "@/components/HelloWorld.vue"; */

export default {
  name: "HomeView",
  components: {
    /* HelloWorld, */
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap");

input:checked ~ .dot {
  transform: translateX(100%);
  background-color: var(--color-primario);
}

h1 {
  font-family: "Indie Flower", cursive;
}
</style>

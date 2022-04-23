<template>
  <nav class="hidden">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Indie+Flower&family=Ubuntu:wght@300&display=swap");

.neonText {
  font-family: "Indie Flower", cursive;
  color: #fff;
  text-shadow: 0 0 7px #fff, 0 0 10px #fff, 0 0 21px #fff, 0 0 42px #8450f5,
    0 0 82px #8450f5, 0 0 92px #8450f5, 0 0 102px #8450f5, 0 0 151px #8450f5;
}

.element {
  background: rgb(11, 9, 28);
  background: url("https://www.transparenttextures.com/patterns/shattered-dark.png"),
    linear-gradient(
      132deg,
      rgba(11, 9, 28, 1) 0%,
      rgba(54, 93, 243, 1) 30%,
      rgba(95, 52, 163, 1) 72%,
      rgba(11, 9, 28, 1) 100%
    );
  /* background: radial-gradient(circle at 129% 75%, #365df396, transparent 100vw),
    radial-gradient(circle at 40% 60%, #8450f594, transparent 100vw); */
  min-height: 100vh;
}

:root {
  --color-fondo: #0b091c;
  --color-primario: #8450f5;
  --color-secundario: #365df3;
  --color-auxiliar: #fff;
}

.color-primario {
  color: var(--color-primario);
}

.color-secundario {
  color: var(--color-secundario);
}

.color-auxiliar {
  color: var(--color-auxiliar);
}

.color-fondo {
  color: var(--color-fondo);
}

.fondo,
.fondo-fondo {
  background-color: var(--color-fondo);
}
.fondo-primario {
  background-color: var(--color-fondo-primario);
}
.fondo-secundario {
  background-color: var(--color-fondo-secundario);
}
.fondo-auxiliar {
  background-color: var(--color-fondo-auxiliar);
}

#app {
  font-family: "Ubuntu", Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: var(--color-fondo);
  color: var(--color-auxiliar);
  min-height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>

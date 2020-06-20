<template>
  <div id="app">
    <Navbar />
    <router-view />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";

export default {
  components: {
    Navbar
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 1rem;
  font-weight: inherit;
  outline: 0;
  border: none;
  text-decoration: none;

  -webkit-tap-highlight-color: rgba(0, 0, 0, 0.2);

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  &::selection {
    background: #e4be04;
  }
}

h1,
h2,
h3,
h4,
h5,
h6,
a,
button {
  font-family: "Ubuntu Mono", monospace;
}

button {
  user-select: none;
}

p,
li,
span {
  font-family: "Ubuntu", sans-serif;
}

#app {
  width: 100%;
  height: 100vh;
  background: black;
}

.page {
  width: 100%;
  height: 100%;
  background: white;
}
</style>

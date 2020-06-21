<template>
  <div class="nav-container">
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/work">Work</router-link>
      <router-link to="/contact">Contact</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar"
};
</script>

<style lang="scss" scoped>
.nav-container {
  width: 100%;
  z-index: 500;
  height: 56px;
  position: fixed;

  nav {
    background: black;
    float: right;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

    @media screen and (max-width: 600px) {
      width: 100%;
      justify-content: space-around;
    }

    a {
      padding: 0px 32px;
      color: white;
      font-size: 1.2rem;
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      user-select: none;

      @media screen and (max-width: 600px) {
        font-size: 3.4vw;

        width: 25%;
      }
    }

    .router-link-exact-active {
      background: #ffd600;
      color: black;
    }
  }
}
</style>
<template>
  <footer>
    <a href="https://www.instagram.com/codestiancat/">
      <font-awesome-icon :icon="['fab', 'instagram']" />
    </a>
    <!-- <font-awesome-icon :icon="['fab', 'linkedin']" /> -->
    <a href="https://github.com/CodestianCat/">
      <font-awesome-icon :icon="['fab', 'github']" />
    </a>
  </footer>
</template>

<script>
export default {
  name: "CodeFooter"
};
</script>

<style lang="scss" scoped>
footer {
  width: 100%;
  padding: 32px;
  background: rgb(30, 30, 30);

  display: flex;
  justify-content: center;
  align-items: center;

  svg {
    color: white;
    font-size: 2rem;
    margin: 0px 16px;
    cursor: pointer;
  }
}
</style>
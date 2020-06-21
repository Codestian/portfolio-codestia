<template>
  <button :style="{background, color}">
    <slot />
  </button>
</template>

<script>
export default {
  name: "CodeButton",
  props: ["background", "color"]
};
</script>

<style lang="scss" scoped>
button {
  width: max-content;
  padding: 8px 12px;
  cursor: pointer;
  text-transform: uppercase;
  transition: 0.2s;

  &:hover {
    box-shadow: inset 0 -3.25em 0 0 black;
    color: #ffd600;
  }
}
</style>
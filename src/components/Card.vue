<template>
  <div class="card-main-container" :style="{maxWidth: width}">
    <div class="card-container" :style="{paddingTop: aspect}">
      <div class="card-content" :style="{background: cardColor}">
        <div class="card-top">
          <span class="card-name">intro</span>
          <font-awesome-icon :icon="['fas', 'user-plus']" />
        </div>
        <div class="card-slot">
          <slot />
        </div>
        <span class="card-class">hero-card</span>
      </div>
      <div class="card-shadow" :style="{border: '2px solid ' + shadowColor}"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["width", "aspect", "cardColor", "shadowColor"]
};
</script>

<style lang="scss" scoped>
.card-main-container {
  width: 100%;

  .card-container {
    width: 100%;
    position: relative;

    .card-content {
      position: absolute;
      top: 0;
      left: 0;
      width: calc(100% - 12px);
      height: calc(100% - 12px);
      z-index: 1;
      display: flex;
      flex-direction: column;
      padding: 24px;

      .card-top {
        display: flex;
        justify-content: space-between;
        align-items: center;
        .card-name {
          text-transform: uppercase;
          font-family: "Ubuntu Mono", monospace;
          font-weight: bold;
          background: black;
          color: white;
          padding: 4px 8px;
          width: max-content;
          letter-spacing: 1px;
        }

        svg {
          font-size: 1.2rem;
        }
      }

      .card-slot {
        flex: 1 1 auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
      }

      .card-class {
        align-self: center;
        font-family: "Ubuntu Mono", monospace;
        text-transform: uppercase;
        font-size: 0.8rem;
      }
    }

    .card-shadow {
      position: absolute;
      bottom: 0;
      right: 0;
      width: calc(100% - 12px);
      height: calc(100% - 12px);
    }
  }
}
</style>
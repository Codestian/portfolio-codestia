<template>
  <div class="page">
    <section class="section">
      <h1>hi im hakim and im 20 yrs old</h1>
      <h2>my passion and interests are in the fields of IT and Design</h2>
      <h3>i design and build websites that priotize rich user experience</h3>
      <h4>my hobby is DIY and building real life architechure in minecraft</h4>
      <h5>this website is still in progress so pls bear with this low quality about page</h5>
      <CodeButton style="margin-top: 16px;" background="#ffd600">this button does nothing</CodeButton>
    </section>
  </div>
</template>

<script>
import CodeButton from "@/components/CodeButton.vue";

export default {
  name: "About",
  components: { CodeButton }
};
</script>

<style lang="scss" scoped>
.section {
  width: 100%;
  height: 100%;
  background: #212121;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  background-size: 30px 30px;
  background-image: linear-gradient(
      to right,
      rgba(255, 255, 255, 0.05) 1px,
      transparent 1px
    ),
    linear-gradient(to bottom, rgba(255, 255, 255, 0.05) 1px, transparent 1px);

  color: white;

  h1,
  h2,
  h3,
  h4,
  h5 {
    font-family: "ubuntu", Arial !important;
  }
}
</style>
<template>
  <div class="page">
    <section class="hero">
      <Card width="520px" aspect="61.8%" card-color="#ffffff" shadow-color="#ffd600">
        <h1 class="title">
          Hi. I'm Hakim.
          <br />A Web Developer.
        </h1>
        <CodeButton background="#ffd600">Explore my work</CodeButton>
      </Card>
    </section>
    <section class="section">
      <h2>Things I do</h2>
      <div class="section-container">
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#00B0FF"
          shadow-color="#ffffff"
        >
          <h1 class="title">Front-end Web Development</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#78909C"
          shadow-color="#ffffff"
        >
          <h1 class="title">Backend-end Web Development</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#448AFF"
          shadow-color="#ffffff"
        >
          <h1 class="title">Internet Of Things</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#7C4DFF"
          shadow-color="#ffffff"
        >
          <h1 class="title">UI/UX Design</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#ff0266"
          shadow-color="#ffffff"
        >
          <h1 class="title">Graphic Design</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
        <Card
          style="margin:32px 32px 0px 32px;"
          width="400px"
          aspect="60%"
          card-color="#00BFA5"
          shadow-color="#ffffff"
        >
          <h1 class="title">Minecraft</h1>
          <CodeButton background="#ffd600">Learn more</CodeButton>
        </Card>
      </div>
    </section>
    <CodeFooter />
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import CodeButton from "@/components/CodeButton.vue";
import CodeFooter from "@/components/CodeFooter.vue";

export default {
  name: "Home",
  components: { Card, CodeButton, CodeFooter }
};
</script>

<style lang="scss" scoped>
.cardes {
  background: red;
}

.hero {
  width: 100%;
  min-height: 600px;
  height: 100%;
  background: linear-gradient(rgba(33, 33, 33, 0.6), rgba(33, 33, 33, 0.6)),
    url("https://images.unsplash.com/photo-1592191136579-27d0d2d44e86?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1423&q=80");

  background-size: cover;
  background-position: 50% 50%;

  display: flex;
  justify-content: center;
  align-items: center;

  padding: 32px;

  .title {
    font-size: 3rem;
    padding-bottom: 16px;

    @media screen and (max-width: 600px) {
      font-size: 8vw;
    }
  }
}

.section {
  width: 100%;
  background: #212121;
  display: flex;
  flex-direction: column;
  align-items: center;

  background-size: 30px 30px;
  background-image: linear-gradient(
      to right,
      rgba(255, 255, 255, 0.05) 1px,
      transparent 1px
    ),
    linear-gradient(to bottom, rgba(255, 255, 255, 0.05) 1px, transparent 1px);

  h2 {
    color: white;
    font-size: 1.4rem;
    margin-top: 32px;
  }

  .title {
    font-size: 2rem;
    padding-bottom: 12px;

    @media screen and (max-width: 600px) {
      font-size: 5.4vw;
    }
  }

  // padding: 32px;

  .section-container {
    width: 100%;
    height: 100%;
    max-width: 1440px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding-bottom: 32px;
  }
}
</style>
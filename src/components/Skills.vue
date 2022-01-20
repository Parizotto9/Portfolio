<template>
  <div class="skills">
    <section>
      <h1>Skills</h1>
      <img src="./../assets/nuxt.png" alt="Working" />
      <article>
        <p>This are some of the tools that I work with</p>
      </article>
    </section>
    <section>
      <div class="tools">
        <div class="a box"></div>
        <div class="b box"></div>
        <div class="c box"></div>
        <div class="d box"></div>
        <div class="e box"></div>
        <div class="f box"></div>
        <div class="g box"></div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.skills {
  padding: 50px;
  display: flex;
  justify-content: space-around;
  background-color: #a9cadc;
  height: 600px;
  box-shadow: inset 0em 0em 2em 0.5em rgba(0, 0, 0, 0.25);
}
h1 {
  text-align: center;
  font-size: 4rem;
  padding-bottom: 40px;
}
.tools {
  display: grid;
  gap: 15px;
  margin-top: 70px;
  grid-template-columns: repeat(4, 100px);
  grid-template-rows: repeat(4, 100px);
  color: rgb(245, 245, 245);
}
p {
  text-align: center;
  margin-top: 20px;
  inline-size: 300px;
  overflow-wrap: break-word;
  font-weight: 600;
  font-size: 1.3rem;
}
.box {
  border-radius: 20px;
  text-transform: uppercase;
  font-weight: 800;
}
.a {
  background-image: url("./../assets/Js.png");
  background-size: 100%;
  grid-column: 1/3;
  grid-row: 1/3;
}
.b {
  background-image: url("./../assets/restApi.png");
  background-size: 100%;
  grid-column: 3/4;
  grid-row: 1/2;
}
.c {
  background-image: url("./../assets/css.png");
  background-size: 100%;
  grid-column: 3/4;
  grid-row: 2/3;
}
.d {
  background-image: url("./../assets/nuxtt.png");
  background-size: 100%;
  grid-column: 2/3;
  grid-row: 3/4;
}
.e {
  background-image: url("./../assets/html.png");
  background-size: 100%;
  grid-column: 3/4;
  grid-row: 3/4;
}
.f {
  background-image: url("./../assets/vuetify.png");
  background-size: 100%;
  grid-column: 4/5;
  grid-row: 3/4;
}
.g {
  background-image: url("./../assets/vue.png");
  background-size: 100%;
  grid-column: 3/4;
  grid-row: 4/5;
}
</style>

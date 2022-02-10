<template>
  <div class="skills">
    <section>
      <h1>Skills</h1>
      <img src="./../assets/nuxt.png" alt="Working" />
      <article class="desk">
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
    <article class="mob">
      <p>This are some of the tools that I work with</p>
    </article>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@media (max-width: 600px) {
  h1 {
    font-size: 2.8rem;
    padding-bottom: 10px;
  }
  p {
    margin-top: 00px;
  }
  img {
    display: none;
  }
  .skills {
    flex-direction: column;
  }
  .desk {
    display: none;
  }
  .tools {
    gap: 7px;
    grid-template-columns: repeat(4, 65px);
    grid-template-rows: repeat(4, 65px);
  }
}
@media (min-width: 600px) and (max-width: 1200px) {
  .desk {
    display: none;
  }
  p {
    margin-top: 20px;
  }
  h1 {
    font-size: 2.8rem;
    padding-bottom: 10px;
  }
  img {
    display: none;
  }
  .skills {
    flex-direction: column;
    height: 650px;
  }
  .tools {
    gap: 15px;
    grid-template-columns: repeat(4, 100px);
    grid-template-rows: repeat(4, 100px);
  }
}
@media (min-width: 1200px) {
  .tools {
    gap: 15px;
    grid-template-columns: repeat(4, 100px);
    grid-template-rows: repeat(4, 100px);
  }
  .mob {
    display: none;
  }
  h1 {
    font-size: 3.5rem;
    padding-bottom: 40px;
  }
  .skills {
    height: 600px;
  }
  p {
    margin-top: 20px;
  }
}
.skills {
  padding: 50px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  background-color: #a9cadc;

  box-shadow: inset 0em 0em 2em 0.5em rgba(0, 0, 0, 0.25);
}
h1 {
  text-align: center;
}
.tools {
  display: grid;
  margin-top: 20px;
  color: rgb(245, 245, 245);
}
.mob {
  padding-top: 20px;
  padding-bottom: 10px;
}
p {
  text-align: center;
  inline-size: 300px;
  overflow-wrap: break-word;
  font-weight: 600;
  font-size: 1.3rem;
}
.box {
  border-radius: 20px;
  text-transform: uppercase;
  font-weight: 800;
  box-shadow: 10px 10px 8px rgba(0, 0, 0, 0.07);
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

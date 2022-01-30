<template>
  <div class="home">
    <section class="text">
      <p>FrontEnd</p>
      <p>Developer</p>
      <h4>A junior FrontEnd developer searching to grow and learn</h4>
    </section>
    <section>
      <img src="./../assets/svgs/home.svg" alt="home img" class="img" />
    </section>
    <section class="balls">
      <div class="ball"></div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.home {
  margin-top: -250px;
  margin-bottom: 300px;
  position: relative;
  display: flex;
  justify-content: space-between;
}
.img {
  width: 500px;
}
.ball {
  position: absolute;
  width: 400px;
  left: -70px;
  top: -40px;
  height: 400px;
  border-radius: 50%;
  background: linear-gradient(90deg, #152837 5%, #04d7a2 100%);
  filter: blur(10px);
}
.text {
  margin-left: 10%;
  z-index: 1;
}
h4 {
  margin-top: 10px;
  font-weight: 500;
  font-size: 1.2rem;
  inline-size: 300px;
  overflow-wrap: break-word;
}
p {
  font-family: "Gentium Book Basic", serif;
  font-weight: 700;
  font-size: 4.4rem;
  text-shadow: 0 10px 7px rgba(0, 0, 0, 0.07);
}
</style>

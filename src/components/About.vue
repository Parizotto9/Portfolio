<template>
  <div class="about">
    <section>
      <div class="divimg">
        <img class="img" src="./../assets/me.png" alt="Parizotto" />
      </div>
    </section>
    <section style="position: relative">
      <h1 class="title">About</h1>
      <article class="box">
        <p>
          Hello, my name is Daniel Parizotto and I was a civil Engineering
          student, but when the pandemic started, I was so bored that I decided
          to start studying programming, it started as a hobby, but I was too
          excited, and at some point I decided to change my carrer. Now I am
          working with it, and excited with my future as a FrontEnd developer,
          and maybe a FullStack.
        </p>
      </article>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.box {
  position: relative;
  background-color: #a9cadc;
  width: 600px;
  height: 140px;
  padding: 50px;
  border-radius: 25px;
  box-shadow: 0 32px 60px rgba(0, 0, 0, 0.07);
  overflow: hidden;
}
.box::before {
  content: "";
  position: absolute;
  top: -590px;
  left: -15%;
  width: 100%;
  height: 320%;
  background: linear-gradient(90deg, transparent, #7899aa33);
  transform: rotate(71deg);
  pointer-events: none;
  filter: blur(5px);
}
.divimg {
  position: relative;
}
.img {
  position: absolute;
  width: 300px;
  top: 180px;
  left: -210px;
  width: 250px;
  box-shadow: 0 32px 60px rgba(0, 0, 0, 0.07);
  border-radius: 30px 0px 30px 30px;
  z-index: 1;
}
.about {
  display: flex;
  justify-content: end;
  margin-top: 120px;
  margin-right: 10%;
  height: 600px;
}
p {
  font-size: 1.1rem;
}
article {
  position: relative;
}
article .title {
  text-align: center;
}
.title {
  z-index: 1;
  position: absolute;
  left: 0;
  right: 0;
  text-align: center;
  top: -45px;
  font-size: 3.5rem;
  overflow: visible;
}
.menu {
  display: flex;
  justify-items: center;
  justify-content: center;
}
</style>

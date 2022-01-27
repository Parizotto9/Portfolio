<template>
  <div class="about">
    <section>
      <div class="divimg">
        <img class="img" src="./../assets/me.png" alt="Parizotto" />
      </div>
    </section>
    <section class="box">
      <article>
        <h1 class="title">About</h1>
        <p>
          Hello, my name is Daniel Parizotto and I was a civil Engineering
          student, but when the pandemic started, I was so bored that I decided
          to start studying programming, it started as a hobby, but I was too
          excited, and at some point decided to change my carrer. Now I am
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
  background-color: #a9cadc;
  width: 600px;
  height: 110px;
  padding: 40px;
  border-radius: 25px;
  box-shadow: 0 32px 60px rgba(0, 0, 0, 0.07);
}
.divimg {
  position: relative;
}
.img {
  position: absolute;
  width: 300px;
  top: 160px;
  left: -210px;
  width: 250px;
  box-shadow: 0 32px 60px rgba(0, 0, 0, 0.07);
  border-radius: 30px 0px 30px 30px;
}
.about {
  display: flex;
  justify-content: end;
  margin-top: 120px;
  margin-right: 10%;
  height: 600px;
}
h1 {
  font-size: 3rem;
}
p {
  font-size: 1.2rem;
}
article {
  position: relative;
}
article .title {
  text-align: center;
}
.title {
  position: absolute;
  left: 0;
  right: 0;
  top: -70px;
}
.menu {
  display: flex;
  justify-items: center;
  justify-content: center;
}
</style>

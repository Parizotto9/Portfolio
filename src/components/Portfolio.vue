<template>
  <div class="portfolio">
    <section class="text">
      <h1>Portfolio</h1>
      <p>
        I am now working as a freelancer for a brazilian company Projeto
        Internet, as a FrontEnd developer I build responsive and intuitive
        pages. I finished three projects with them, after every single one of
        them I realize how much I learned from it, and I want to continue
        growing and learning everything I can.
      </p>
    </section>
    <section class="imagebox">
      <img src="./../assets/coding.png" alt="Coding" />
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.portfolio {
  display: flex;
  justify-content: center;
  padding-bottom: 100px;
}
h1 {
  text-align: center;
  font-size: 3.5rem;
}
.text {
  padding: 40px;
  margin-top: 100px;
}
.imagebox {
  margin-top: 80px;
}
p {
  text-align: center;
  margin-top: 20px;
  inline-size: 550px;
  overflow-wrap: break-word;
  font-size: 1.1rem;
}
</style>

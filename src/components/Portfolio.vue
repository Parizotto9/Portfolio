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
@media (max-width: 600px) {
  p {
    font-size: 0.92rem;
    inline-size: 290px !important;
  }
  h1 {
    font-size: 2.8rem;
  }
  .portfolio {
    flex-direction: column;
    align-items: center;
  }
  img {
    width: 300px;
  }
}
@media (min-width: 600px) and (max-width: 1000px) {
  .portfolio {
    flex-direction: column;
    align-items: center;
  }
  h1 {
    font-size: 2.8rem;
  }
}
@media (min-width: 1000px) and (max-width: 1200px) {
  h1 {
    font-size: 2.8rem;
  }
  .text {
    padding: 15px;
  }
}
@media (min-width: 1200px) {
  h1 {
    font-size: 3.5rem;
  }
  p {
    font-size: 1.1rem;
  }
  .text {
    padding: 40px;
  }
}
.portfolio {
  display: flex;
  justify-content: center;
  padding-bottom: 100px;
}
h1 {
  text-align: center;
}
.text {
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
}
</style>

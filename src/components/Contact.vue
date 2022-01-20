<template>
  <div class="contact">
    <section>
      <h1>Contact me</h1>
    </section>
    <section class="sect">
      <div class="img">
        <img src="./../assets/logo.png" alt="" />
        <ul>
          <li>
            <a href="mailto:parizottojs@gmail.com">
              <i class="fa fa-envelope"></i>
            </a>
          </li>
          <li>
            <a href="tel:+55 (81) 997652428">
              <i class="fa fa-phone"></i>
            </a>
          </li>
          <li>
            <a
              href="https://www.linkedin.com/in/daniel-parizotto-34b18a1b1/"
              target="_blank"
            >
              <i class="fa fa-linkedin"></i>
            </a>
          </li>
          <li>
            <a href="https://github.com/Parizotto9" target="_blank">
              <i class="fa fa-github"></i>
            </a>
          </li>
        </ul>
      </div>
      <div class="text">
        <p>
          Please send me a message, any criticizes, compliments or advices just
          let me know that you visited my website, it will make me very happy
        </p>
        <div class="place">
          <div class="placeicon">
            <i class="fas fa-map-marker-alt"></i>
          </div>
          Recife, Pernambuco - Brazil
        </div>
      </div>
    </section>
    <section class="footer">
      <p>Designed by</p>
      <p>© Parizotto</p>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.contact {
  justify-content: center;
  text-align: center;
  padding: 50px;
  background-color: #a9cadc;
  position: relative;
}
.footer {
  position: absolute;
  right: 0;
  left: 0;
  bottom: 0px;
  background-color: #04d7a2;
}
.sect {
  display: flex;
  justify-content: space-around;
  margin-top: 50px;
  padding-bottom: 30px;
}
p {
  font-size: 1.3rem;
}
ul {
  display: flex;
  margin-top: 30px;
}
a {
  color: #04d7a2;
}
li {
  transition: 0.6s;
  color: #04d7a2;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #152837;
  height: 30px;
  width: 30px;
  border-radius: 80px;
  margin-left: 10px;
  list-style: none;
  box-shadow: 0 5px 4px rgba(0, 0, 0, 0.3);
}
li:hover {
  transition: 0.6s;
  transform: translateY(-10px);
}
li:nth-child(1):hover a {
  color: #e4405f;
  transition: 0.6s;
}
li:nth-child(2):hover a {
  color: #25d366;
  transition: 0.6s;
}
li:nth-child(3):hover a {
  color: #0a66c2;
  transition: 0.6s;
}
li:nth-child(4):hover a {
  transition: 0.6s;
  color: #007bb6;
}
h1 {
  font-size: 2.5rem;
}
.place {
  font-size: 1.1rem;
  margin-top: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.placeicon {
  margin-right: 10px;
  display: flex;
  background-color: #152837;
  border-radius: 50%;
  align-items: center;
  justify-content: center;
  height: 30px;
  width: 30px;
  color: #04d7a2;
  box-shadow: 0 5px 4px rgba(0, 0, 0, 0.3);
}
.text {
  inline-size: 400px;
  overflow-wrap: break-word;
}
img {
  width: 100px;
}
</style>

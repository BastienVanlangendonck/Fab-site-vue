<template>
  <footer class="footer-container">
    <div class="img-container">
      <img src="../assets/logo-250.png" alt="Logo" />
      <a href="https://www.facebook.com/fabienne.ferrari.79"
        ><i class="fab fa-facebook-square fa-2x"
      /></a>
    </div>
    <div class="contact">
      <h3 class="contact-title">Contact</h3>
      <p class="adresse">Place jean jaures<br />26100 romans sur isere</p>
      <a class="mailto" href="mailto:san@antonio.net">Envoyez moi un mail</a>
    </div>
  </footer>
</template>

<script>
export default {
  name: "footer",
};
</script>

<style scoped>
.footer-container {
  display: flex;
  position: relative;
  align-items: center;
  width: 100%;
  background: rgb(44, 21, 76);
  background: linear-gradient(
    90deg,
    rgba(44, 21, 76, 1) 65%,
    rgba(113, 73, 151, 1) 100%
  );
}

img {
  width: 100px;
  height: 100px;
}

i {
  margin-left: 1rem;
  color: rgba(194, 194, 194, 0.575);
}

i:hover {
  cursor: pointer;
}

.img-container {
  position: absolute;
  margin-left: 1rem;
  display: flex;
  align-items: flex-end;
}

.contact {
  text-align: center;
  margin: auto;
}

.mailto {
  text-decoration: none;
  color: white;
  font-size: 1.3rem;
}

.mailto:hover {
  text-decoration: underline;
  font-size: 1.5rem;
  transition: 0.5s ease all;
}

.contact-title {
  font-size: 1.5rem;
  text-transform: uppercase;
}
</style>

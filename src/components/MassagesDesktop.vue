<template>
  <div class="banner">
    <img src="../assets/massages.png" alt="massages-image" class="banner-img" />
    <h2 class="banner-title">Les Massages</h2>
  </div>

  <div class="description-card">
    <h3 class="title">Massage Metamorphique</h3>
    <div class="story">
      <h4 class="chapter">Un peu d'histoire</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "MassagesDesktop",
};
</script>

<style scoped>
.banner {
  display: flex;
  position: relative;
  margin: 8rem 0rem 1rem 0rem;
  min-height: 6.5rem;
  background-color: #643f8a;
  box-shadow: rgba(0, 0, 0, 0.315) 0px 10px 20px,
    rgba(0, 0, 0, 0.363) 0px 6px 6px;
}

.banner-title {
  align-self: center;
  margin: auto;
  font-size: 2rem;
}

.banner-img {
  position: absolute;
  left: 250px;
  height: 85px;
  width: 175px;
  margin: 0.5rem;
}

.description-card {
  background-color: #653f8ad5;
  box-shadow: rgba(0, 0, 0, 0.315) 0px 10px 20px,
    rgba(0, 0, 0, 0.363) 0px 6px 6px;
  padding: 1rem;
  margin-bottom: 1rem;
}

.title {
  text-align: center;
  text-transform: uppercase;
  width: 300px;
  margin: auto;
  background: rgb(44, 21, 76);
  background: linear-gradient(
    90deg,
    rgba(44, 21, 76, 1) 65%,
    rgba(113, 73, 151, 1) 100%
  );
  box-shadow: rgba(255, 255, 255, 0.35) 0px 5px 15px;
}

.chapter {
  text-align: center;
}
</style>

<template>
  <div class="cars">
    <div class="nav">
      <ul>
        <li>
          <router-link to="/" class="link link--metis">Home</router-link>
        </li>
        <li>
          <router-link to="/about" class="link link--metis">About</router-link>
        </li>
      </ul>
    </div>
    <div id="container">
      <div>
        <img src="../assets/media/images/porschelogo.png" alt="logo porsche">
      </div>
      <div>
        <img id="bugatti" src="../assets/media/images/bugattilogo.png" alt="logo bugatti">
      </div>
      <div>
        <img src="../assets/media/images/lamborghinilogo.png" alt="logo lamborghini">
      </div>
      <div class="porsche">
        <ul>
          <li>
            <router-link to="/cars/porsche-911">Porsche 911</router-link>
          </li>
        </ul>
      </div>
      <div class="bugatti">
        <ul>
          <li>
            <router-link to="/cars/bugatti-eb110">Bugatti EB110</router-link>
          </li>
        </ul>
      </div>
      <div class="lamborghini">
        <ul>
          <li>
            <router-link to="/cars/lamborghini-diablo">Lamborghini Diablo</router-link>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Cars",
}

</script>

<style scoped>
.nav {
  width: 100%;
}

.nav ul {
  padding: 30px;
  justify-content: start;
}

.nav ul li {
  margin: 0 25px;
  font-size: 1.55rem;
}

.nav ul {
  display: flex;
  justify-content: start;
}

#container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 0.4fr 1fr;
  gap: 25px 0;
  margin: 5% 15% 0;
}

#container div:nth-child(-n +3) {
  display: flex;
  justify-content: center;
  align-items: center;
}

#container img {
  width: 40%;
}

#bugatti {
  width: 50%!important;
}

</style>
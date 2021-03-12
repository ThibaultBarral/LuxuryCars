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
    <div class="all">
      <div class="container">
        <div class="top">
          <div class="content">
            <img src="../assets/media/images/porschelogo.png" alt="logo porsche">
            <ul>
              <li>
                <router-link to="/cars/porsche-911">Porsche 911</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <img src="../assets/media/images/lamborghinilogo.png" alt="logo lamborghini">
            <ul>
              <li>
                <router-link to="/cars/lamborghini-diablo">Lamborghini Diablo</router-link>
              </li>
            </ul>
          </div>
        </div>
        <div class="bottom">
          <div class="content">
            <img src="../assets/media/images/bugattilogo.png" alt="logo bugatti">
            <ul>
              <li>
                <router-link to="/cars/bugatti-eb110">Bugatti EB110</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <img src="../assets/media/images/fordlogo.png" alt="logo ford">
            <ul>
              <li>
                <router-link to="/cars/ford-gt40">Ford GT40</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <img id="ferrari" src="../assets/media/images/ferrarilogo.png" alt="logo ferrari">
            <ul>
              <li>
                <router-link to="/cars/ferrari-f40">Ferrari F40</router-link>
              </li>
            </ul>
          </div>
        </div>
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

.all {
  display: flex;
  align-items: center;
  justify-content: center;
  height: calc(100vh - 40px - 85px);
}

.container {
  margin: 10px;
  width: 100%;
}

.top , .bottom {
  display: flex;
  justify-content: center;
  width: 100%;
}

.top div {
  margin: 10px;
  display: flex;
  border: 1px solid black;
  height: 10vh;
  width: 25%;
}

.bottom div {
  margin: 10px;
  display: flex;
  border: 1px solid black;
  height: 10vh;
  width: 30%;
}

.top img {
  width: 10%;
}

.bottom img {
  width: 15%;
}

.content {
  padding: 5px 5px 5px 10px;
  display: flex;
  align-items: center;
  border-radius: 8px;
}

#ferrari {
  width: 11%;
}

.content li {
  margin: 10px;
}

@media screen and (max-width: 979px) {
  .top div {
    width: 50%;
  }
}

@media screen and (max-width: 699px) {
  .top {
    flex-direction: column;
  }
  .top div {
    width: auto;
  }
  .bottom {
    flex-direction: column;
  }
  .bottom div {
    width: auto;
  }
  .nav {
    width: auto;
  }
  .nav li {
    font-size: 20px!important;
  }
}

@media screen and (max-width: 499px) {
  .nav ul {
    justify-content: center;
  }
}

</style>
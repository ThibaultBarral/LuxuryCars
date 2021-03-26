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
            <router-link to="/cars/porsche-911">
              <img src="../assets/media/images/porschelogo.png" alt="logo porsche">
            </router-link>
            <ul>
              <li>
                <router-link to="/cars/porsche-911">Porsche 911</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <router-link to="/cars/lamborghini-diablo">
            <img src="../assets/media/images/lamborghinilogo.png" alt="logo lamborghini">
            </router-link>
            <ul>
              <li>
                <router-link to="/cars/lamborghini-diablo">Lamborghini Diablo</router-link>
              </li>
            </ul>
          </div>
        </div>
        <div class="bottom">
          <div class="content">
            <router-link to="/cars/bugatti-eb110">
            <img src="../assets/media/images/bugattilogo.png" alt="logo bugatti">
            </router-link>
            <ul>
              <li>
                <router-link to="/cars/bugatti-eb110">Bugatti EB110</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <router-link to="/cars/ford-gt40">
            <img src="../assets/media/images/fordlogo.png" alt="logo ford">
            </router-link>
            <ul>
              <li>
                <router-link to="/cars/ford-gt40">Ford GT40</router-link>
              </li>
            </ul>
          </div>
          <div class="content">
            <router-link to="/cars/ferrari-f40">
            <img id="ferrari" src="../assets/media/images/ferrarilogo.png" alt="logo ferrari">
            </router-link>
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
  font-size: 1.1rem;
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
  width: 3vw;
}

.bottom img {
  width: 6vw;
}

#ferrari {
  width: 3vw;
}

.content {
  padding: 5px 5px 5px 10px;
  display: flex;
  align-items: center;
  border-radius: 8px;
}

#app > div > div.all > div > div.top > div > a {
  display: contents;
}

#app > div > div.all > div > div.bottom > div > a {
  display: contents;
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
  .top img {
    width: 6vw;
  }
  .bottom img {
    width: 12vw;
  }
  #ferrari {
    width: 6vw;
  }
}

@media screen and (max-width: 499px) {
  .nav ul {
    justify-content: center;
  }
  .top img {
    width: 12vw;
  }
  .bottom img {
    width: 24vw;
  }
  #ferrari {
    width: 12vw;
  }
}

</style>
<template>
  <div class="home">
    <div class="display">
      <nav>
        <h1>Luxury cars</h1>
      </nav>
    </div>
    <div class="left">
      <div class="top">
        <img src="../assets/media/images/porsche911.jpg" alt="porsche 911">
      </div>
      <div>
        <nav>
          <ul>
            <li>
              <router-link to="/" class="link link--metis">Home</router-link>
            </li>
            <li>
              <router-link to="/cars" class="link link--metis">Cars</router-link>
            </li>
            <li>
              <router-link to="/about" class="link link--metis">About</router-link>
            </li>
          </ul>
        </nav>
        <img id="shelby" src="../assets/media/images/shelby.jpg" alt="shelby cobra">
        <div class="text">
          <p>The Reference Website</p>
          <p>For Luxury Cars</p>
        </div>
      </div>
    </div>
    <div class="right">
      <h1>Luxury Cars</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
}
</script>

<style scoped>
.home {
  display: flex;
  margin: 10px;
  height: calc(100vh - 60px);
}

.left {
  width: 90%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.right {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 10%;
}

.right h1 {
  font-size: 3.55rem;
  letter-spacing: 20px;
  text-transform: uppercase;
  writing-mode: vertical-rl;
  transform: rotate(180deg);
}

.top {
  display: flex;
  justify-content: center;
  margin: 10px 0 10px 0;
}

.display nav h1 {
  font-size: 3.55rem;
  letter-spacing: 20px;
  text-transform: uppercase;
}

.display nav {
  padding-bottom: 10px;
}

nav, ul {
  display: flex;
}

.left nav {
  justify-content: flex-end;
  margin-right: 25%;
}

li {
  padding: 0 40px;
}

.text {
  padding: 40px;
}

img {
  width: 55%;
}

#shelby {
  width: 100%;

}

@media screen and (max-width: 1279px) {
  .right {
    display: none;
  }
  .left {
    width: 100%;
  }
  .home {
    flex-direction: column;
  }
}

@media screen and (min-width: 1280px) {
  .display {
    display: none;
  }
}

@media screen and (max-width: 979px) {
  .left nav {
    margin-right: 0;
    justify-content: center;
  }
}

@media screen and (max-width: 654px) {
  .display nav h1 {
    font-size: 2.15rem;
  }
}

@media screen and (max-width: 519px) {
  .display nav h1 {
    font-size: 1.57rem;
  }
  .display nav {
    justify-content: center;
  }
  .top {
    display: none;
  }
  .left nav {
    margin: 30px;
  }
  .home {
    height: 0;
  }
}

@media screen and (min-width: 520px) {
  #shelby {
    display: none;
  }
}

@media screen and (max-width: 445px) {
  .display nav h1 {
    text-align: center;
  }
}

@media screen and (max-width: 370px) {
  .left nav ul {
    flex-direction: column;
  }
  .left nav {
    text-align: center;
  }
  .left nav ul li {
    margin: 10px;
  }
}

</style>
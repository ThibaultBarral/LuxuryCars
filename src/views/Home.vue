<template>
  <div class="home">
    <div id="display">
      <h1>Luxury Cars</h1>
      <div id="container">
        <div class="top">
          <img class="porsche" src="../assets/media/images/porsche911.jpg" alt="porsche 911">
          <img class="maserati" src="../assets/media/images/maserati-300-sl-papillon.jpg" alt="maserati 330sl">
        </div>
        <div class="bottom">
          <div>
            <ul>
              <li>
                <router-link to="/cars" class="link link--metis">Cars</router-link>
              </li>
              <li>
                <router-link to="/about" class="link link--metis">About</router-link>
              </li>
            </ul>
          </div>
          <div>
            <img class="ac-cobra" src="../assets/media/images/ac-cobra.jpg" alt="ac-cobra">
            <img class="classic" src="../assets/media/images/porscheclassic.jpg" alt="porsche 911">
          </div>
        </div>
      </div>
    </div>
    <div class="left">
      <h1>Luxury Cars</h1>
      <div class="rightflex">
        <img class="porsche" src="../assets/media/images/porsche911.jpg" alt="porsche 911">
        <div>
          <ul>
            <li>
              <router-link to="/cars" class="link link--metis">Cars</router-link>
            </li>
            <li>
              <router-link to="/about" class="link link--metis">About</router-link>
            </li>
          </ul>
          <img class="maserati" src="../assets/media/images/maserati-300-sl-papillon.jpg" alt="maserati 330sl">
        </div>
      </div>
    </div>
    <div class="right">
      <ul>
        <li>
          <router-link to="/cars" class="link link--metis">Cars</router-link>
        </li>
        <li>
          <router-link to="/about" class="link link--metis">About</router-link>
        </li>
      </ul>
      <img class="ac-cobra" src="../assets/media/images/ac-cobra.jpg" alt="ac-cobra">
      <img class="classic" src="../assets/media/images/porscheclassic.jpg" alt="porsche 911">
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
}
</script>

<style scoped>
ul {
  display: flex;
}

div > ul > li {
  margin: 0 4%;
}

.left ul {
  display: flex;
  justify-content: flex-end;
  padding: 10px;
  font-size: 1.28rem;
  width: 100%;
}

h1 {
  font-size: 2.45rem;
  margin: 5% 0 0 7%;
}

.home {
  display: flex;
}

.left, .right {
  width: 50%;
}

.right {
  display: flex;
  flex-direction: column;
  padding: 10px 10px 10px 0;
  justify-content: center;
  height: calc(100vh - 60px);
}

.right img:nth-child(1) {
  margin-top: -7%;
}

.left img:nth-child(1) {
  margin-top: 7%;
}

.left {
  display: flex;
  flex-direction: column;
  padding: 10px 0 10px 10px;
}

.rightflex {
  display: flex;
  align-items: flex-end;
  flex-direction: column;
}

.rightflex div:nth-child(2) {
  display: flex;
  justify-content: flex-end;
}


.right ul {
  display: flex;
  justify-content: flex-start;
  padding: 10px;
  font-size: 1.28rem;
}

.ac-cobra {
  width: 60%;
}

.maserati {
  width: 35%;
}

.porsche {
  width: 62%;
}

.classic {
  width: 42%;
}

#display {
  display: flex;
  flex-direction: column;
}

#container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-top: 10px solid black;
  padding: 10px;
  margin-top: 4%;
  background-color: #C9B17E;
  min-height: calc(100vh - 39px - 40px);
}

#container img {
  width: 30%;
  border: 2px solid black;
}

.top {
  display: flex;
  width: 100%;
  justify-content: center;
}

.top img {
  margin: 0 8px 8px 8px;
}

.bottom {
  display: flex;
  font-size: 1.45rem;
}

.bottom img {
  margin: 0 8px 8px 8px;
}

.bottom div {
  display: flex;
  width: 100%;
}

.bottom div:nth-of-type(1) {
  justify-content: center;
  align-items: center;
}

@media screen and (max-width: 956px) {
  .left ul {
    display: none;
  }
}

@media screen and (min-width: 957px) {
  .right ul {
    display: none;
  }
}

@media screen and (max-width: 899px) {
  .left {
    display: none;
  }
  .right {
    display: none;
  }
}

@media screen and (min-width: 898px) {
  #display {
    display: none;
  }
  #container {
    display: none;
  }
}

@media screen and (max-width: 610px) {
  .bottom {
    display: flex;
    flex-direction: column;
  }
  #container img {
    width: 40%!important;
  }
  .bottom div:nth-of-type(1) {
    margin: 3% 0;
  }
  .bottom img {
    margin: 8px!important;
  }
  .top img {
    margin: 8px!important;
  }
  .bottom div:nth-of-type(2) {
    justify-content: center;
  }
}

</style>
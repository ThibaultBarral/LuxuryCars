<template>
  <div class="about">
    <div id="left" class="xLarge-2 large-2 medium-12 small-12 xSmall-12">
      <div class="xLarge-2 large-2 medium-12 small-12 xSmall-12">
        <h1>Luxury Cars</h1>
      </div>
      <div class="xLarge-10 large-10 medium-12 small-12 xSmall-12">
        <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
          Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
          congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
          suscipit tortor eget felis porttitor volutpat.</p>
        <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
          Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
          congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
          suscipit tortor eget felis porttitor volutpat.</p>
        <div class="line"></div>
        <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
          Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
          congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
          suscipit tortor eget felis porttitor volutpat.</p>
        <div class="line"></div>
        <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
          Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
          congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
          suscipit tortor eget felis porttitor volutpat.</p>
        <div class="line"></div>
      </div>
    </div>
    <div id="right" class="xLarge-10 large-10 medium-12 small-12 xSmall-12">
      <nav>
        <ul>
          <li>
            <router-link to="/" class="link link--metis">Home</router-link>
          </li>
          <li>
            <router-link to="/cars" class="link link--metis">Cars</router-link>
          </li>
        </ul>
        <div class="titleright">
          <h1>The Reference Website For Luxury Cars</h1>
        </div>
      </nav>
      <div class="bottom">
        <div class="xLarge-6 large-6 medium-12 small-12 xSmall-12">
            <div class="lineleft"></div>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Vivamus
              suscipit tortor eget felis porttitor volutpat. Curabitur non nulla sit amet nisl
              tempus convallis quis ac lectus. Nulla porttitor accumsan tincidunt. Nulla porttitor
              accumsan tincidunt. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.</p>
            <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
              Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
              congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
              suscipit tortor eget felis porttitor volutpat.</p>
            <div class="lineleft"></div>
            <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
              Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
              congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
              suscipit tortor eget felis porttitor volutpat.Quisque velit nisi, pretium ut
              lacinia in, elementum id enim. Mauris blandit aliquet elit, eget tincidunt
              nibh pulvinar a. Donec rutrum congue leo eget malesuada. Donec rutrum congue
              leo eget malesuada. Vivamus suscipit tortor eget felis porttitor volutpat.</p>
            <div class="lineleft"></div>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Vivamus
              suscipit tortor eget felis porttitor volutpat. Curabitur non nulla sit amet nisl
              tempus convallis quis ac lectus. Nulla porttitor accumsan tincidunt. Nulla porttitor
              accumsan tincidunt. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.</p>
        </div>
        <div class="xLarge-6 large-6 medium-12 small-12 xSmall-12">
          <img src="../assets/media/images/porsche911grey.jpg" alt="porsche grey">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About"
}
</script>

<style scoped>
.about {
  color: #FDE0A1;
  display: flex;
  min-height: calc(100vh - 40px);
}

#left {
  background-color: #6B5D50;
  display: flex;
}

#left div:nth-child(1) {
  display: flex;
  align-items: center;
}

#left h1 {
  font-size: 37px;
  letter-spacing: 20px;
  text-transform: uppercase;
  writing-mode: vertical-rl;
  transform: rotate(180deg);
}

#left p {
  font-size: 12px;
  margin: 10px;
  width: calc(100% - 20px);
  text-align: justify;
}

.line {
  margin: 10px;
  width: calc(100% - 20px);
  height: 1px;
  background-color: #FDE0A1;
}

#right {
  padding: 10px;
  border-left: 20px solid black;
  background-color: #2C2216;
}

nav {
  display: flex;
  width: 100%;
  flex-direction: column;
}

ul {
  display: flex;
  justify-content: flex-end;
}

li {
  margin: 0 10px;
}

.titleright {
  padding: 15px 0;
}

#right h1 {
  font-size: 40px;
}

.lineleft {
  margin: 4px 40% 4px 0;
  width: 75%;
  height: 1px;
  background-color: #FDE0A1;
}

.bottom {
  display: flex;
  min-height: calc(100vh - 40px - 20px - 16px - 70px);
}

#right > div > div:nth-child(1) {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

#right > div > div:nth-child(1) p {
  margin: 10px 0;
  width: calc(100% - 20px);
  text-align: justify;
}

#right > div > div:nth-child(2) {
  display: flex;
  justify-content: center;
  align-items: center;
}

img {
  width: 50vh;
  padding: 10px;
}

@media screen and (max-width: 1279px) {
  .about {
    flex-direction: column;
  }
  #left {
    width: 100%;
    flex-direction: column;
  }
  #left div:nth-child(1) {
    width: 100%;
    padding-top: 10px;
    justify-content: center;
    text-align: center;
  }
  #left h1 {
    font-size: 2.15rem;
    writing-mode: horizontal-tb;
    transform: none;
  }
  #left div:nth-child(2) {
    width: 100%;
  }
  .line {
    display: flex;
  }
  #right {
    width: 100%;
    padding: 0;
    border: 0;
  }
  #right h1 {
    margin: 0;
  }
  ul {
    padding: 10px;
  }
  .titleright {
    padding: 10px;
  }
  #right > div > div:nth-child(1) {
    padding: 10px;
  }
}

@media screen and (max-width: 779px) {
  .bottom {
    flex-direction: column;
  }
  .bottom div:nth-child(2) {
    width: auto;
    margin: 10px;
  }
}

@media screen and (max-width: 519px) {
  img {
    width: 70vw;
  }
}


@media screen and (max-width: 489px) {
  #left h1 {
    font-size: 1.15rem;
  }
  #right h1 {
    font-size: 2rem;
  }
}

</style>
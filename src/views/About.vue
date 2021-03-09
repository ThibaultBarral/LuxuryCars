<template>
  <div class="about">
    <div class="left">
      <div>
        <h1>Luxury Cars</h1>
      </div>
      <div>
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
        <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
          Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
          congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
          suscipit tortor eget felis porttitor volutpat.</p>
        <div class="line"></div>
      </div>
    </div>
    <div class="right">
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
      <div class="containerbottom">
        <div class="bottom">
          <div class="leftbottom">
            <div class="lineright"></div>
            <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
              Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
              congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
              suscipit tortor eget felis porttitor volutpat.</p>
            <p>Quisque velit nisi, pretium ut lacinia in, elementum id enim.
              Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Donec rutrum
              congue leo eget malesuada. Donec rutrum congue leo eget malesuada. Vivamus
              suscipit tortor eget felis porttitor volutpat.Quisque velit nisi, pretium ut
              lacinia in, elementum id enim. Mauris blandit aliquet elit, eget tincidunt
              nibh pulvinar a. Donec rutrum congue leo eget malesuada. Donec rutrum congue
              leo eget malesuada. Vivamus suscipit tortor eget felis porttitor volutpat.</p>
            <div class="lineright"></div>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus. Vivamus
              suscipit tortor eget felis porttitor volutpat. Curabitur non nulla sit amet nisl
              tempus convallis quis ac lectus. Nulla porttitor accumsan tincidunt. Nulla porttitor
              accumsan tincidunt. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.</p>
          </div>
          <div>
            <img src="../assets/media/images/porsche911grey.jpg" alt="porsche grey">
          </div>
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

.left {
  display: flex;
  width: 25%;
  background-color: #6B5D50;
}

.left div:nth-child(1) {
  width: 20%;
  display: flex;
  align-items: center;
}

.left div:nth-child(2) {
  width: 80%;
}

.left h1 {
  font-size: 4rem;
  letter-spacing: 20px;
  text-transform: uppercase;
  writing-mode: vertical-rl;
  transform: rotate(180deg);
}

.left p {
  font-size: 11px;
  padding: 10px;
}

.line {
  margin: 10px;
  height: 1px;
  background-color: #FDE0A1;
}

.right {
  padding: 10px;
  width: 75%;
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
  padding: 10px 0;
}

.right h1 {
  font-size: 3rem;
  margin-right: 30%;
}

.containerbottom {
  height: calc(100% - 132px);
  display: flex;
  justify-content: flex-end;
}

.bottom {
  display: flex;
}

.lineright {
  margin: 4px 40% 4px 0;
  height: 1px;
  background-color: #FDE0A1;
}

.leftbottom {
  width: 48%;
  margin: 2% 0;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}

.bottom div:nth-child(1) p {
  font-size: 12px;
  padding: 10px 0;
  margin-right: 40%;
}

.bottom div:nth-child(2) {
  width: 52%;
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
}

.bottom img {
  width: 60%;
}

</style>
<template>
  <div class="home">
    <h1>Luxury Cars</h1>
    <img id="911" src="../assets/media/images/porsche911.jpg" alt="porsche911">
    <img id="cobra" src="../assets/media/images/ac-cobra.jpg" alt="ac-cobra">
    <img id="classic" src="../assets/media/images/porscheclassic.jpg" alt="porscheclassic">
    <div>
      <ul>
        <li>
          <router-link to="/cars">Cars</router-link>
        </li>
        <li>
          <router-link to="/about">About</router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
}
</script>

<style scoped>
div > ul {
  padding: 10px;
}

div > ul > li {
  margin: 0 20px;
}

ul {
  display: flex;
  justify-content: start;
}

h1 {
  font-size: 2.45rem;
  margin: 5% 0 0 7%;
}

</style>
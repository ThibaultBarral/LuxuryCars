<template>
  <footer>
    <div class="linefooter"></div>
    <ul>
      <li>
        <router-link to="/" class="link link--metis">Home</router-link>
      </li>
    </ul>
  </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
footer {
  flex-direction: column;
  display: flex;
  align-items: center;
  margin: 0 0 1% 0;
}

.linefooter {
  margin-bottom: 6px;
  height: 1px;
  width: 10%;
  background-color: black;
}
</style>
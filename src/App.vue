<template>
  <div id="app">
    <Home />
    <router-view />
  </div>
</template>

<style>
@import url(assets/css/responsive.css);
@import url(assets/css/reboot.css);

@font-face {
  font-family: "Source Code Pro";
  src: url("/assets/fonts/Source_Code_Pro");
}

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: #E1DED5;
  color: #020102;
  border: 20px solid #020102;
  min-height: 100vh;
}


/*=============================================================
                            LINK
=============================================================*/
.link {
  position: relative;
}

.link::before,
.link::after {
  position: absolute;
  width: 100%;
  height: 1px;
  background-color: #707070;
  top: 100%;
  left: 0;
}

.link::before {
  content: '';
}

.link--metis {
  text-transform: uppercase;
}

.link--metis::before {
  transform-origin: 100% 50%;
  transform: scale3d(0, 1, 1);
  transition: transform 0.3s;
}

.link--metis:hover::before {
  transform-origin: 0% 50%;
  transform: scale3d(1, 1, 1);
}

</style>

<template>
  <div class="lamborghinidiablo">
    <div class="left">
      <div class="columnleft">
        <div class="textitalic">
          <p>Sed porttitor lectus nibh. Proin eget tortor risus.
            Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.
            Vivamus magna justo, lacinia eget consectetur sed, convallis at
            tellus. Vestibulum ante ipsum primis in faucibus orci luctus et
            ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet
            aliquam vel, ullamcorper sit amet ligula.</p>
        </div>
        <div>
          <img src="../assets/media/images/lamborghinidiablo.jpg" alt="lamborghini diablo">
        </div>
      </div>
      <div>
        <p>A Criminal Life</p>
        <div class="text">
          <p>Vestibulum ac diam sit amet quam vehicula elementum sed sit
            amet dui. Curabitur aliquet quam id dui posuere blandit. Vestibulum ac
            diam sit amet quam vehicula elementum sed sit amet dui. Vestibulum ac diam
            sit amet quam vehicula elementum sed sit amet dui. Vivamus magna justo, lacinia
            eget consectetur sed, convallis at tellus.</p>
          <p>Proin eget tortor risus. Donec sollicitudin molestie malesuada.
            Donec rutrum congue leo eget malesuada. Cras ultricies ligula sed magna
            dictum porta.</p>
        </div>
      </div>
    </div>
    <div class="right">
      <div>
        <p>A Criminal Life</p>
        <div class="text">
          <p>Vestibulum ante ipsum primis in faucibus orci luctus
            et ultrices posuere cubilia Curae; Donec velit neque, auctor
            sit amet aliquam vel, ullamcorper sit amet ligula. Donec sollicitudin
            molestie malesuada. Vivamus magna justo, lacinia eget consectetur sed,
            convallis at tellus.</p>
          <p>Vestibulum ac diam sit amet quam vehicula elementum sed sit amet
            dui. Praesent sapien massa, convallis a pellentesque nec, egestas
            non nisi.</p>
        </div>
      </div>
      <div class="columnright">
        <img src="../assets/media/images/diablo.jpg" alt="lamborghini diablo">
        <div class="text">
          <p class="textitalic">Pellentesque in ipsum id orci porta dapibus. Lorem ipsum dolor
            sit amet, consectetur adipiscing elit. Vestibulum ac diam sit amet quam
            vehicula elementum sed sit amet dui. Nulla quis lorem ut libero malesuada feugiat.</p>
          <h1>Luxury Cars : The
            perfect Vehicle for
            Money Launderers</h1>
          <p>Nulla porttitor accumsan tincidunt. Nulla quis
            lorem ut libero malesuada feugiat. Donec sollicitudin molestie
            malesuada. Quisque velit nisi, pretium ut lacinia in, elementum id
            enim. Curabitur non nulla sit amet nisl tempus convallis quis ac lectus.
            Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.</p>
        </div>
        <Footer />
      </div>
    </div>
  </div>
</template>

<script>
import Footer from "@/components/Footer";
export default {
  components: {Footer}
}

</script>

<style scoped>
.lamborghinidiablo {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  grid-column-gap: 10%;
}

.left, .right {
  margin: 10px;
}

.left {
  display: grid;
  grid-template-columns: 1.5fr 0.5fr;
  grid-template-rows: 1fr;
  grid-column-gap: 20px;
}

.left div:nth-child(2) {
  flex-direction: column;
  display: flex;
  justify-content: flex-end;
}

.left img {
  width: 100%;
}

.right {
  display: grid;
  grid-template-columns: 0.5fr 1.5fr;
  grid-template-rows: 1fr;
  grid-column-gap: 20px;
}

.columnright {
  flex-direction: column;
}

.columnleft {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto 1.5fr;
}

.columnleft div:nth-child(2) {
  display: grid;
  flex-direction: column;
  align-items: flex-end;
}

.right img {
  width: 100%;
}

.columnright > .text {
  margin-right: 20%;
}

.textitalic {
  font-size: 10px;
  font-style: italic;
  padding: 18px 0 10px 0;
}

.text h1 {
  padding-top: 10px;
  font-size: 1.8rem;
}

.text p:nth-child(odd) {
  font-size: 10px;
  padding: 20px 0;
}
.text p:nth-child(2) {
  font-size: 10px;
  padding-top: 20px;
}

@media screen and (max-width: 1100px) {
  .columnleft div:nth-child(2) {
    display: grid;
    flex-direction: column;
    align-items: flex-start;
  }
  .left div:nth-child(2) {
    flex-direction: column;
    display: flex;
    justify-content: flex-start;
  }
}

@media screen and (max-width: 979px) {
  .lamborghinidiablo {
    display: block;
  }
}

@media screen and (max-width: 669px) {
  .left div:nth-child(2) {
    flex-direction: column;
    display: flex;
    justify-content: flex-end;
  }
}

@media screen and (max-width: 519px) {
  .left {
    display: block;
  }
  .left div:nth-child(2) p:nth-child(1) {
    margin-top: 10px;
  }
}

</style>
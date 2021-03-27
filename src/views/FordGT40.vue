<template>
  <div class="fordgt40">
    <div class="left xLarge-6 large-6 medium-12 small-12 xSmall-12">
      <div class="xLarge-8 large-8 medium-8 small-12 xSmall-12">
        <div class="textitalic">
          <p>Sed porttitor lectus nibh. Proin eget tortor risus.
            Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a.
            Vivamus magna justo, lacinia eget consectetur sed, convallis at
            tellus. Vestibulum ante ipsum primis in faucibus orci luctus et
            ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet
            aliquam vel, ullamcorper sit amet ligula.</p>
        </div>
        <div>
          <img src="../assets/media/images/portraitfordtest.jpg" alt="ford gt40">
        </div>
      </div>
      <div class="xLarge-4 large-4 medium-4 small-12 xSmall-12">
        <h2>A Criminal Life</h2>
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
    <div class="right xLarge-6 large-6 medium-12 small-12 xSmall-12">
      <div class="xLarge-4 large-4 medium-4 small-12 xSmall-12">
        <h2>A Criminal Life</h2>
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
      <div class="xLarge-8 large-8 medium-8 small-12 xSmall-12">
        <img src="../assets/media/images/ford.jpg" alt="ford gt40">
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
.fordgt40 {
  display: flex;
  min-height: calc(100vh - 40px);
}

.left, .right {
  margin: 10px;
  width: calc(100% - 20px);
}

.left {
  display: flex;
}

.left div:nth-child(2) {
  flex-direction: column;
  display: flex;
  justify-content: flex-end;
}

#app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-8.large-8.medium-8.small-12.xSmall-12 {
  display: grid;
}

.left img {
  width: 100%;
}

.right img {
  width: 100%;
}

.right {
  display: flex;
}

.textitalic {
  font-size: 0.875rem;
  font-style: italic;
  padding: 10px 0;
  text-align: justify;
}

.text h1 {
  padding-top: 0.625rem;
  font-size: 1.8rem;
  padding: 20px;
}

h2 {
  font-size: 1.2rem;
  font-weight: 600;
  padding: 0 20px 5px 20px;
}

.text p:nth-child(odd) {
  font-size: 0.9375rem;
  padding: 20px;
  text-align: justify;
  line-height: 1.125;
}

.text p:nth-child(2) {
  font-size: 0.9375rem;
  padding: 0 20px 0 20px;
  text-align: justify;
  line-height: 1.125;
}

.right .textitalic {
  font-size: 0.875rem;
  padding-left: 0!important;
  font-style: italic;
  padding: 10px 0;
  text-align: justify;
}

.right .text h1 {
  padding-top: 0.625rem;
  padding-left: 0!important;
  font-size: 1.8rem;
  padding: 15px;
}

.right h2 {
  font-size: 1.2rem;
  padding-left: 0!important;
  font-weight: 600;
  padding: 0 20px 5px 20px;
}

.right .text p:nth-child(odd) {
  font-size: 0.9375rem;
  padding-left: 0!important;
  padding: 20px;
  text-align: justify;
  line-height: 1.125;
}

.right .text p:nth-child(2) {
  font-size: 0.9375rem;
  padding-left: 0!important;
  padding: 0 20px 20px 20px;
  text-align: justify;
  line-height: 1.125;
}


@media screen and (max-width: 1600px) {
  .fordgt40 > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-8.large-8.medium-12.small-12.xSmall-12 > div:nth-child(2) {
    height: calc(100% - 56px);
  }
  .textitalic {
    font-size: 0.575rem;
  }
  .text p:nth-child(2) {
    font-size: 0.71rem;
  }
  .text p:nth-child(odd) {
    font-size: 0.71rem;
  }
  .right .textitalic {
    font-size: 0.575rem;
  }
  .right .text p:nth-child(2) {
    font-size: 0.71rem;
  }
  .right .text p:nth-child(odd) {
    font-size: 0.71rem;
  }
}

@media screen and (max-width: 1279px) {
  .fordgt40 {
    display: flex;
    flex-direction: column;
  }
}

@media screen and (max-width: 759px) {
  .left {
    display: flex;
  }
  .left div:nth-child(2) p:nth-child(1) {
    margin-top: 10px;
  }
  #app > div > div.left > div:nth-child(2) > h2 {
    padding-top: 10px!important;
  }
}

@media screen and (max-width: 629px) {
  .left {
    flex-direction: column;
  }
  #app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-8.large-8.medium-8.small-12.xSmall-12 {
    width: 100%!important;
  }
  #app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-4.large-4.medium-4.small-12.xSmall-12 {
    width: 100%;
  }
  #app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-4.large-4.medium-4.small-12.xSmall-12 > h2 {
    padding: 0 0 5px 0;
  }
  #app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-4.large-4.medium-4.small-12.xSmall-12 > div > p:nth-child(1) {
    padding: 20px 0 20px 0;
  }
  #app > div > div.left.xLarge-6.large-6.medium-12.small-12.xSmall-12 > div.xLarge-4.large-4.medium-4.small-12.xSmall-12 > div > p:nth-child(2) {
    padding: 0 0 20px 0;
  }

}

</style>
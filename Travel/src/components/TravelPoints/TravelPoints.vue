<template>
  <div class="travels point col-md-3 img">
    <div class="travel content df">
      <div class="travel-image df">
        <img v-for="img in travelImage" :key="img" :src="img.src" :alt="img.alt" />
      </div>
      <div class="travel-text">
        <span class="travel-media">Travelers Point</span>
        <h2>We help to find your dream place</h2>
        <p class="text info mg20">Lorem ipsum dolor sit amet, consectetur adipiscing elit ut aliquam, purus sit amet
          luctus venenatis, lectus
          magna fringilla urna, porttitor rhoncus dolor purus non enim praesent elementum facilisis leo, vel fringilla est
          ullamcorper eget nulla facilisi</p>
        <div class="travel-number">
          <div class="number1 info1">
            <label class="number1">100+</label>
            <span class="number1-text">Holiday Package</span>
            <label class="number1">68</label>
            <span class="number1-text">Elite Transportation</span>
          </div>
          <div class="number2 info2">
            <label class="number2">172</label>
            <span class="number2-text">Hotel</span>
            <label class="number2">32M+</label>
            <span class="number2-text">we help to find your dream place</span>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import "./style.css";
var image1 = ('/src/assets/travel1.png');
var image2 = ('/src/assets/travel2.png');
var image3 = ('/src/assets/travel3.png');
export default {
  data() {
    return {
      travelImage: [
        { src: image1, alt: "travel1" },
        { src: image2, alt: "travel2" },
        { src: image3, alt: "travel3" },
      ]
    }
  }
}
</script>
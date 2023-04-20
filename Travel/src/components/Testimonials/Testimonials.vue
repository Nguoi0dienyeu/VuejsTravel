<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div id="testimonial">
    <span class="top-des-first">
      <p>Testimonial</p>
    </span>
    <h3 class="top-des-second">
      What they say about us
    </h3>
  </div>
  <div class="testimonial-say-about">
    <div class="say-about">
      <div class="about-us">
        <div v-for="iabout in listItemAboutUs" :key="iabout" class="person-us">
          <div class="about-us-header">
            <img :src="iabout.src" :alt="iabout.alt" />
            <p class="header-left">{{ iabout.header }}</p>
          </div>
          <p class="person-text-left">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Doloribus labore hic iusto nulla eaque enim
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script scoped>
import './style.css';
var about1 = ('/src/assets/about1.png');
var about2 = ('/src/assets/about1.png');
var about3 = ('/src/assets/about1.png');
var about4 = ('/src/assets/about1.png');
var about5 = ('/src/assets/about1.png');
var about6 = ('/src/assets/about1.png');
export default {
  data() {
    return {
      listItemAboutUs: [
        { src: about1, alt: "about1", header: "Hammer" },
        { src: about2, alt: "about1", header: "Hammer" },
        { src: about3, alt: "about1", header: "Hammer" },
        { src: about4, alt: "about1", header: "Hammer" },
        { src: about5, alt: "about1", header: "Hammer" },
        { src: about6, alt: "about1", header: "Hammer" },
      ]
    }
  }
}
</script>
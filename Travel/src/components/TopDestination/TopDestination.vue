<template>
  <div id="top-destination">
    <span class="top-des-first">
      <p>Top Destination</p>
    </span>
    <h3 class="top-des-second">
      Discover your love
    </h3>
  </div>
  <div class="discover-desination">
    <div class="detail-descover">
      <div class="detail-image" v-for="items in listItemImage" :key="items">
        <img :src="items.src" :alt="items.alt" />
        <div class="detail-text">
          <p class="detail-top">
            {{ items.title }}
          </p>
          <div class="detail-subtext">
            <p class="sub1">{{ items.subname }}</p>
            <p class="sub2">{{ items.price }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script scoped>
import './style-top.css';
var anh1 = ('/src/assets/anh1.png');
var anh2 = ('/src/assets/anh2.png');
var anh3 = ('/src/assets/anh3.png');
var anh4 = ('/src/assets/anh4.png');
var anh5 = ('/src/assets/anh5.png');
var anh6 = ('/src/assets/anh6.png');
export default {
  data() {
    return {
      listItemImage: [
        { src: anh1, alt: "anh1", title: "Taman Nasional Komodo", subname: "7 days for trips", price: "Rp. 7,5jt" },
        { src: anh2, alt: "anh2", title: "Taman Nasional Bunaken", subname: "9 days for trips", price: "Rp. 10,5jt" },
        { src: anh3, alt: "anh3", title: "Raja Ampat, Papua Barat", subname: "14 days for trips", price: "Rp. 20,5jt" },
        { src: anh4, alt: "anh4", title: "Kepulauan Wakatobi", subname: "12 days for trips", price: "Rp. 9,5jt" },
        { src: anh5, alt: "anh5", title: "Gili Trawangan, Lombok", subname: "7 days for trips", price: "Rp. 6,5jt" },
        { src: anh6, alt: "anh6", title: "Taman Nasional Bromo", subname: "7 days for trips", price: "Rp. 9,5jt" },
      ]
    }
  }
}
</script>

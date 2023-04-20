<script>
import NavigationItem from "./components/Navbar/NavigationItem.vue";
import HeroTitle from "./components/HeroContent/HeroTitle.vue";
import TravelPoints from "./components/TravelPoints/TravelPoints.vue";
import TopDesination from "./components/TopDestination/TopDestination.vue";
import Testimonials from "./components/Testimonials/Testimonials.vue";
import Footer from "./components/Footer/Footer.vue";
export default {
  components: {
    NavigationItem,
    HeroTitle,
    TravelPoints,
    TopDesination,
    Testimonials,
    // eslint-disable-next-line vue/no-reserved-component-names
    Footer,
  }
}

</script>
<template>
  <div id="main-app">
    <div class="nav2 top main-app">
      <NavigationItem />
      <HeroTitle />
    </div>
    <TravelPoints />
    <TopDesination />
    <Testimonials />
    <Footer />
  </div>
</template>
<style scoped>
#main-app {
  height: auto;
}

.nav2.top.main-app {
  font-size: 12px;
  min-height: 720px;
  padding: 0 2rem;
  color: #ffffff;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.25)),
    url("./assets/Background.png");
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
}
</style>

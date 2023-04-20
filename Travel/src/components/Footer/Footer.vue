<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="footer">
    <div class="footer-content">
      <div class="footer-logo">
        <span>travelplan</span>
        <p class="footer-bottom">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat, minima illum laboriosam dicta ipsum quis
          commodi incidunt omnis molestias optio amet eveniet error !
        </p>
      </div>
      <div class="menu-foo">
        <p class="link-menus-text">links</p>
        <ul class="link-item-menu" v-for="mitems in linkItemFooter" :key="mitems">
          <li class="sub-link"><a class="sub-link-active" href="" :id="`item-${mitems}`" :type="mitems">{{ mitems
          }}</a></li>
        </ul>
      </div>
      <div class="menu-foo">
        <p class="service-menus-text">services</p>
        <ul class="ser-item-menu" v-for="sitem in listServiceFooter" :key="sitem">
          <li class="sub-link"><a class="sub-link-active" href="" :id="`item-${sitem}`" :type="sitem">{{ sitem
          }}</a></li>
        </ul>
      </div>
      <div class="menu-foo">
        <p class="contact-text">contact</p>
        <div class="contact-info">
          <p>Address: Cầu giấy - Dịch Vọng Hậu - TP Hà Nội</p>
          <p>Sson, Age 28</p>
          <p>Phone: 84 9742 808 76</p>
          <p>Email: mr.itproduction@gmail.com</p>
          <p>Maps: VietNam, Ha Noi</p>
        </div>
      </div>
      <div class="menu-foo">
        <p>Socials</p>
        <div class="social-image">
          <a href=""><img v-for="isocial in listSocials" :key="isocial" :src="isocial.src" :alt="isocial.alt" /></a>
        </div>
      </div>
    </div>

  </div>
</template>
<script scoped>
import "./style.css";
var ins = ('/src/assets/ins.png');
var fb = ('/src/assets/fb.png');
var tw = ('/src/assets/tw.png');
var pr = ('/src/assets/pr.png');
var git = ('/src/assets/git.png');
export default {
  data() {
    return {
      linkItemFooter: [
        'Discover',
        'Special Deals',
        'Services',
        'Community',
        'About us',
      ],
      listServiceFooter: [
        'About us',
        'Blog & Articles',
        'Term and Condition',
        'Privacy Policy',
        'Contact us',
      ],
      listSocials: [
        { src: ins, alt: 'ins' },
        { src: fb, alt: 'fb' },
        { src: tw, alt: 'tw' },
        { src: pr, alt: 'pr' },
        { src: git, alt: 'git' },
      ]
    }
  }
}
</script>
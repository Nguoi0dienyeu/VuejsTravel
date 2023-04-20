<template>
  <div id="header-nav">
    <header>
      <div class="logo">
        <span>travelplan</span>
      </div>
      <div class="menus">
        <ul class="item-menus" v-for="item in listItemNavigation" :key="item">
          <li class="active"><a class="navigation-link" href="" :id="`item-${item}`" :type="item">{{ item }}</a></li>
        </ul>
      </div>
      <div class="language-top col">
        <select class="form-select" aria-label="Default select example">
          <option class="lang-first" selected value="0"><label>VN</label></option>
          <option value="1"><label>EN</label></option>
          <option value="2"><label>IN</label></option>
          <option value="3"><label>FR</label></option>
        </select>
      </div>
      <div class="menu-mobile top col">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" fill="currentColor" class="bi bi-list"
          viewBox="0 0 16 16">
          <path fill-rule="evenodd"
            d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z" />
        </svg>
      </div>
    </header>
  </div>
</template>
<script scoped>
import './nav.css';
export default {
  data() {
    return {
      listItemNavigation: [
        'Home',
        'Discover',
        'Services',
        'News',
        'About Us',
        'Contact'
      ]
    }
  }
};
</script>
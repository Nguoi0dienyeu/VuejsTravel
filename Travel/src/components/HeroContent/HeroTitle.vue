<template>
  <div id="hero">
    <div class="hero-title">
      <span class="hero-header">
        <p>Explore the world with a smile</p>
      </span>
      <span class="hero-info">
        <p>
          Lorem ipsum dolor sit amet,consectetur adipiscing elit ut aliquam,
          purus sit amet luctus venenatis, lectus magna fringilla urna,
          porttitor rhoncus dolor purus non enim praesent elementum facilisis
          leo,
        </p>
      </span>
    </div>
    <div class="hero-search">
      <!-- <span class="city-input-group"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" color="black"
            fill="currentColor" class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
            <path d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z" />
          </svg></span> -->
      <div class="input-group mb-3">
        <input list="allcountry" class="form-control" placeholder="City in Desitination"
          v-on:change="onChangInputDataList()" />
        <datalist id="allcountry">
          <option v-for="icoun in allcountry" :key="icoun">{{ icoun }}</option>
        </datalist>
        <input class="form-control" v-for="item in itemType" :key="item" :id="`type-${item}`" :type="item"
          placeholder="Person" :value="0" />
        <button id="find-tour">
          <span class="find-tour text">Find trip now</span>
        </button>
      </div>
    </div>
  </div>
</template>
<script>
import "./hero.css";
// eslint-disable-next-line @typescript-eslint/no-unused-vars
import { ref } from "vue";
export default {
  data() {
    return {
      allcountry: [],
      defaultValuePerson: 0,
      itemType: ["date", "number"]
    }
  },
  // methods: {
  //   onChangInputDataList(e) {
  //     const listItem = ref([]);
  //     async function getData() {
  //       const response = await fetch("https://vietjetcms-api.vietjetair.com/api/v1/country?languageId=a6ca5a9f-6a9c-4f35-bf1c-c42ea3d62f14&requestId=KFG4NUJKGV1C-1679365426238");
  //       const result = await response.json();
  //       listItem.value = result.countries;
  //       console.log('result', result.countries[0].countryName);
  //     }
  //     getData();
  //   }
  // }
  // created() {
  //   fetch(
  //     "https://vietjetcms-api.vietjetair.com/api/v1/country?languageId=a6ca5a9f-6a9c-4f35-bf1c-c42ea3d62f14&requestId=KFG4NUJKGV1C-1679365426238"
  //   )
  //     .then((res) => res.json())
  //     .then((res) => {
  //       this.countries = res.results;
  //       console.log("results", res.results)
  //     })
  // }
}

</script>

<template>
  <div class="layout-default"> 
    <mt-header fixed title="Kuka food">
      <router-link to="/" slot="left">
        <mt-button icon="back">
          Back
        </mt-button>
      </router-link>
    </mt-header>
    <p>
      Okay this is testing
    </p>
    <div>
      <Nuxt />
    </div>
    <mt-tabbar v-model="selected" fixed :selected.sync="selected">
      <mt-tab-item id="tab1">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#home" />
        </svg>
        <!-- <small>
          Главная
        </small>  -->
      </mt-tab-item>
      <mt-tab-item id="tab2">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#home" />
        </svg>
        <!-- <img slot="icon" src="../assets/house.svg"> -->
        <!-- <small>
          Главная
        </small>  -->
      </mt-tab-item>
      <mt-tab-item id="tab3">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#home" />
        </svg>
        <!-- <img slot="icon" src="../assets/house.svg"> -->
        <!-- <small>
          Главная
        </small>  -->
      </mt-tab-item>
      <mt-tab-item id="tab4">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#profile" />
        </svg>
        <!-- <img slot="icon" src="../assets/house.svg"> -->
        <!-- <small>
          Профиль
        </small>  -->
      </mt-tab-item>
    </mt-tabbar>
  </div>  
</template>

<script>
// import Header from 'mint-ui'
export default {
  name: 'default',
  data() {
    return {
      selected: 'tab1'
    }
  },
  components: {
    // Header
  }
}
</script>

<style>
p {
  font-family: 'Source Sans Pro';
}
</style>
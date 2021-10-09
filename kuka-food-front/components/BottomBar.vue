<template>
  <mt-tabbar v-model="selected" fixed :selected.sync="selected">
      <mt-tab-item id="tab1">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#home" />
        </svg>
        <small>
          🏡 Главная
        </small> 
      </mt-tab-item>
      <mt-tab-item id="tab2">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#heart-circle" />
        </svg>
        <small>
          💔 Избранное
        </small> 
      </mt-tab-item>
      <mt-tab-item id="tab3">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#map" />
        </svg>
        <small>
          🗺 Карта
        </small> 
      </mt-tab-item>
      <mt-tab-item id="tab4">
        <svg slot="icon" class="ic-16 ic-primary" >
          <use xlink:href="~/assets/sprite.svg#profile" />
        </svg>
        <small>
          👨🏻 Профиль
        </small> 
      </mt-tab-item>
    </mt-tabbar>  
</template>

<script>
export default {
  data () {
    return {
      selected: 'tab1',
      routes: [
        {
          id: 'tab1',
          route: '/'
        },
        {
          id: 'tab2',
          route: '/favorite'
        },
        {
          id: 'tab3',
          route: '/map'
        },
        {
          id: 'tab4',
          route: '/profile'
        },
      ]
    }
  }
}
</script>

<style>

</style>
<template>
  <div class="layout-default"> 
    <Header />
    <div class="layout-content">
      <Nuxt />
    </div>
    <BottomBar /> 
  </div>  
</template>

<script>
export default {
  name: 'default',
  head: {
    title: 'Home page',
    meta: [
      { name: 'viewport', content: 'width=device-width, user-scalable=no' },
    ],
  },
  data() {
    return {
    }
  },
}
</script>

<style lang="scss">
  .layout-default {
    font-family: $font-family;
  }
  .layout-content {
    // margin-top: 40px;
    padding: 10px 5px;
  }
</style>
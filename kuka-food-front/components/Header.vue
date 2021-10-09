<template>
  <div class="header">
    <div class="header__left">
      <Icon size="25" icon="back"  fill="white" />
    </div>
    <div class="header__center">
      <Search />
    </div>
    <div class="header__right">
      <!-- <Icon size="25" icon="back"  fill="white" /> -->
    </div>
  </div>
  <!-- <mt-header fixed>
      <router-link to="/" slot="left">
        <mt-button icon="back">
          Back
        </mt-button>
      </router-link>
      <div>

      </div>
    </mt-header>   -->
</template>

<script>
export default {
  data() {
    return {
      search: ''
    }
  },
}
</script>

<style lang="scss" scoped>
  .header {
    background: $primary-bg;
    color: $color;
    justify-content: space-between;
    padding: 10px;
    align-items: center;
    display: flex;
    &__left {
      display: flex;
    }
    &__center {
      margin-left: 10px;
      margin-right: 10px;
      width: 100%;
    }
  }
</style>
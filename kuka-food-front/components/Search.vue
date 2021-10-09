<template>
<div class="fixed">
  <div class="search">
    <input class="search__input" type="search" placeholder="Жан плов Лагман" />
  </div>  
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.fixed {
  position: sticky;
  top: 0;
}
.search {
  position: relative;
  &__input {
    border:none;
    width: 100%;
    height: 30px;
    border-radius: 2px;
    padding: 5px;
    &:focus {
      outline: 1px  solid $primary-bg;
    }
  }
}

</style>
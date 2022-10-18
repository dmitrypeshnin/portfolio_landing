<template>
  <header class="header">
    <h1>Dmitriy Novik</h1>
    <div class="container">
      <nav class="header__menu menu">
        <div class="menu__items">
          <a href="" class="menu__link" v-for="item in items" :key="item">{{ item }}</a>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderBlock",
  data() {
    return {
      items: ["Home", "About me", "Skills", "Portfolio", "Contacts" ]
    }
  }
};
</script>

<style lang="scss" scoped>
  // style reset
  @import '../../node_modules/css-reset-and-normalize/scss/reset-and-normalize.scss';
  @import '../../node_modules/css-reset-and-normalize/scss/link-reset.scss';
  @import '../../node_modules/css-reset-and-normalize/scss/button-reset.scss';
  
  .container {
    max-width: 945px;
  }
</style>

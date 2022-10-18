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
  .container {
    max-width: 945px;
  }
</style>

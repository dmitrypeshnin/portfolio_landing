<template>
  <header class="header">
    <div class="header__inner">
      <nav class="header__menu menu">
        <ul class="menu__list">
          <li class="menu__item" v-for="item in menuList" :key="item.text">
            <a class="menu__link" :href="item.linkPath">{{ item.text }}</a>
          </li>
        </ul>
    </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderBlock",
  data() {
    return {
      menuList: [
        {
          text: "Home",
          linkPath: "#",
        },
        {
          text: "About me",
          linkPath: "#"
        },{
          text: "Skills",
          linkPath: "#"
        },
        {
          text: "Portfolio",
          linkPath: "#"
        },
        {
          text: "Contacts",
          linkPath: "#"
        }
      ]
    }
  }
};
</script>


<style lang="scss" scoped>
.header {
  &__inner {
    max-width: 945px;
    margin: 0 auto;
  }
  &__menu {
    height: 88px;
    border-bottom: 1px solid #828282;
    line-height: 88px;
  }
}

.menu {
  &__list {
    display: flex;
    justify-content: space-between;
  }
  &__link {
    font-family: 'Gilroy-Bold';
    font-size: 18px;
    line-height: 22px;
    color: #828282;
  }
  &__link-active {
    color: #070707;
  }
}
</style>

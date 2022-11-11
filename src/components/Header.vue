<template>
  <header class="header">
    <div class="container">
      <nav class="header__menu menu">
        <ul class="menu__list">
          <li class="menu__item">
            <a href="#" class="menu__link menu__link-active">Home</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">About me</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">Skills</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">Portfolio</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">Contacts</a>
          </li>
        </ul>
    </nav>
    </div>
    
  </header>
</template>

<script>
export default {
  name: "HeaderBlock"
};
</script>


<style lang="scss" scoped>
.container {
  max-width: 945px;
  margin: 0 auto;
}
.header {
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

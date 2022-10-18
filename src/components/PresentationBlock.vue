<template>
  <div class="presentationBlock">
    <div class="container">
      <div class="presentationBlock__top">
        <div class="presentationBlock__name">Denis Novik</div>
        <div class="presentationBlock__title">UX | UI designer 24 years old, Minsk</div>
        <div class="presentationBlock__lang lang-switcher">
          <a class="lang-switcher__eng lang-switcher__eng-active">ENG</a>
          <a class="lang-switcher__ru">RU</a>
          
          
          
        </div>
      </div>
      <div class="presentationBlock__bottom">
        <img src="../assets/img/photo.png" alt="photo">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PresentationBlock',
  props: {
    msg: String
  }
}
</script>

<style lang="scss" scoped>
.container {
  width: 945px;
  margin: 0 auto;
}

.presentationBlock {
  &__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 0 54px 0;
  }

  &__name {
    width: 124px;
    font-family: 'Gilroy-Bold';
    font-size: 48px;
    color: #070707;
  }

  &__title {
    width: 156px;
    font-family: 'Gilroy-Medium';
    font-size: 18px;
    color: #070707;
  }
}

.lang-switcher {
  display: flex;
  flex-direction: column-reverse;
  font-family: 'Gilroy-Bold';
  font-size: 16px;
  color: #828282;
  transform: rotate(-180deg);
  

  &__eng {
    border-top: 1px solid #000000;
    padding-top: 6px;
    writing-mode: vertical-lr;
    cursor: pointer;
  }

  &__ru {
    border-bottom: 1px solid #000000;
    padding-bottom: 6px;
    writing-mode: vertical-lr;
    cursor: pointer;
  }

  &__eng-active {
    color: #000000;
  }
}
</style>

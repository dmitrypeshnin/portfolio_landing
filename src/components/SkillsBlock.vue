<template>
    <div class="skillsBlock">
      <div class="skillsBlock__inner">
        <h2 class="skillsBlock__title">Skills</h2>
        <p class="skillsBlock__text">I work in such programs as</p>
        <div class="skillsBlock__program-levels program-levels">
          <div class="program-levels__item" v-for="item in skills" v-bind:key="item.title" >
            <img class="program-levels__app-icon" :src="item.img" :alt="item.title" >
            <p class="program-levels__app-title">{{ item.title }}</p>
            <img class="program-levels__star" :src="item.imgStars" :alt="item.title">
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: "SkillsBlock",
  data () {
    return {
      skills: [
        {
          img: require('@/assets/img/photoshop-icon.png'),
          title: 'Adobe Photoshop',
          imgStars: require('@/assets/img/photoshop-rating.png')
        },
        {
          img: require('@/assets/img/illustrator-icon.png'),
          title: 'Adobe Illustrator',
          imgStars: require('@/assets/img/illustrator-rating.png')
        },
        {
          img: require('@/assets/img/after-effects-icon.png'),
          title: 'Adobe After Effects',
          imgStars: require('@/assets/img/after-effects-rating.png')
        },
        {
          img: require('@/assets/img/figma-icon.png'),
          title: 'Figma',
          imgStars: require('@/assets/img/figma-rating.png')
        },
      ]
    }
  },
};
</script>

<style lang="scss" scoped>
  .skillsBlock {
    &__inner {
      height: 610px;
      padding-top: 91px;
      margin: 0 auto;
    }
    &__title {
      text-align: center;
      margin-bottom: 70px;
      font-family: 'Gilroy-Bold';
      font-size: 34px;
      line-height: 42px;
      color: #070707;
    }
    &__text {
      text-align: center;
      margin-bottom: 83px;
      font-family: 'Gilroy-Medium';
      font-size: 18px;
      line-height: 22px;
      color: #070707;
    }
  }

  .program-levels {
    display: flex;
    justify-content: center;

    &__item {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-left: 90px;
      &:first-child {
        margin-left: 0;
      }
    }
    &__app-icon {
      height: 90px;
      margin-bottom: 24px;
    }
    &__app-title {
      height: 27px;
      width: min-content;
      margin-bottom: 40px;
      text-align: center;
      font-family: 'Gilroy-Bold';
      font-size: 14px;
      line-height: 17px;
      color: #828282;
    }
  }
</style>

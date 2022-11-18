<template>
    <div class="skillsBlock">
      <div class="skillsBlock__inner">
        <h2 class="skillsBlock__title">Skills</h2>
        <p class="skillsBlock__text">I work in such programs as</p>
        <div class="skillsBlock__program-levels program-levels">
          <div
            v-for="item of skills"
            :key="item.title"
            class="program-levels__item"
          >
            <img class="program-levels__app-icon" :src="item.img" :alt="item.title">
            <p class="program-levels__app-title">{{ item.title }}</p>
            <div class="program-levels__stars">
            <div
              v-for="stars in 5"
              :key="stars.title"
            >
              <img class="program-levels__star" :src="item.imgStar" :alt="item.title">
            </div>
            </div>
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
          id: 1,
          img: require('@/assets/img/photoshop-icon.png'),
          title: 'Adobe Photoshop',
          imgStar: require('@/assets/img/dark-star.png')
        },
        {
          id: 2,
          img: require('@/assets/img/illustrator-icon.png'),
          title: 'Adobe Illustrator',
          imgStar: require('@/assets/img/dark-star.png')
        },
        {
          id: 3,
          img: require('@/assets/img/after-effects-icon.png'),
          title: 'Adobe After Effects',
          imgStar: require('@/assets/img/dark-star.png')
        },
        {
          id: 4,
          img: require('@/assets/img/figma-icon.png'),
          title: 'Figma',
          imgStar: require('@/assets/img/dark-star.png')
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
      margin-left: 160px;
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
    &__stars {
      display: flex;
    }
  }

  .stars {
    min-width: 100%;
    display: flex;
    justify-content: space-between;
  }
</style>

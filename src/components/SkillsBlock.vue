<template>
    <div class="skillsBlock">
      <div class="skillsBlock__inner">
        <h2 class="skillsBlock__title">Skills</h2>
        <p class="skillsBlock__text">I work in such programs as</p>
        <div class="skillsBlock__program-levels program-levels">
          <div class="program-levels__item">
            <img class="program-levels__app-icon" src="../assets/img/photoshop-icon.png" alt="photoshop-icon">
            <h3 class="program-levels__app-title">Adobe<br>Photoshop</h3>
            <div class="program-levels__stars stars">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/light-star.png" alt="light-star">
            </div>
          </div>
          <div class="program-levels__item">
            <img class="program-levels__app-icon" src="../assets/img/illustrator-icon.png" alt="illustrator-icon">
            <h3 class="program-levels__app-title">Adobe<br>Illustrator</h3>
            <div class="program-levels__stars stars">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/light-star.png" alt="light-star">
              <img class="stars__star-item" src="../assets/img/light-star.png" alt="light-star">
            </div>
          </div>
          <div class="program-levels__item">
            <img class="program-levels__app-icon" src="../assets/img/after-effects-icon.png" alt="after-effects-icon">
            <h3 class="program-levels__app-title">Adobe<br>After Effects</h3>
            <div class="program-levels__stars stars">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/light-star.png" alt="light-star">
            </div>
          </div>
          <div class="program-levels__item">
            <img class="program-levels__app-icon" src="../assets/img/figma-icon.png" alt="figma-icon">
            <h3 class="program-levels__app-title">Figma</h3>
            <div class="program-levels__stars stars">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/dark-star.png" alt="dark-star">
              <img class="stars__star-item" src="../assets/img/light-star.png" alt="light-star">
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: "SkillsBlock"
};
</script>

<style lang="scss" scoped>
  .skillsBlock {
    &__inner {
      max-width: 935px;
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
    justify-content: space-between;
    
    &__item {
      width: 166px;
      display: flex;
      flex-direction: column;
      align-items: center;

    }
    &__app-icon {
      height: 90px;
      margin-bottom: 24px;
    }
    &__app-title {
      height: 27px;
      margin-bottom: 40px;
      text-align: center;
      font-family: 'Gilroy-Bold';
      font-size: 14px;
      line-height: 17px;
      color: #828282;
    }
  }

  .stars {
    min-width: 100%;
    display: flex;
    justify-content: space-between;
  }
</style>
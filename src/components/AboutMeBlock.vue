<template>
  <div class="about">
    <h2 class="about__title">About me</h2>
    <div class="about__text">
      <p class="about__text-item">
        Hi, I'm Denis – UX/UI designer from Minsk.
        <br>
        I'm interested in design and everything connected with it.
      </p>
      <p class="about__text-item">
        I'm studying at courses "Web and mobile design
        <br>
        interfaces" in IT-Academy.
      </p>
      <p class="about__text-item">
        Ready to implement excellent projects
        <br>
        with wonderful people.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
}
</script>

<style lang="scss" scoped>
  .about {
    max-width: 100%;
    height: 506px;
    background: #F6F6F6;
    color: #070707;
    padding-top: 120px;
    &__title {
      margin: 0 auto;
      font-family: 'Gilroy-Bold';
      font-size: 34px;
      line-height: 42px;
      text-align: center;
      margin-bottom: 18px;
    }
    &__text {
      max-width: 485px;
      margin: 0 auto;
      text-align: center;
      font-family: 'Gilroy-Medium';
      font-size: 18px;
      line-height: 22px;
    }
    &__text-item {
      margin-bottom: 55px;
    }
  }
</style>

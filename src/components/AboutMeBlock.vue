<template>
  <div class="about">
    <div class="about__title">
      <h1>About me</h1>
    </div>
    <div class="about__desc">
      <p class="about__text">
        Hi, I'm Denis – UX/UI designer from Minsk.
        <br>
        I'm interested in design and everything connected with it.
        </p>
      <p class="about__text">
        I'm studying at courses "Web and mobile design
        <br>
        interfaces" in IT-Academy.</p>
      <p class="about__text">Ready to implement excellent projects with wonderful people.</p>
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
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    max-width: 100%;
    height: 506px;
    background: #F6F6F6;
    &__title {
      font-family: 'Gilroy-Bold';
      font-size: 34px;
      line-height: 42px;
      color: #070707;
      margin-bottom: 18px;
    }
    &__text {
      margin-bottom: 55px;
      text-align: center;
    }
  }
  .title {
  }

</style>

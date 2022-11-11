<template>
  <div id="app">
    <Header />
    <PresentationBlock />
    <AboutMeBlock />
  </div>
</template>

<script>
import Header from "@/components/Header";
import PresentationBlock from "@/components/PresentationBlock";
import AboutMeBlock from "@/components/AboutMeBlock";

export default {
  name: 'App',
  components: {
    Header,
    AboutMeBlock,
    PresentationBlock,
  }
}
</script>

<style lang="scss" scoped>
  // reset styles
  @import url('./../node_modules/css-reset-and-normalize/scss/reset-and-normalize.scss');
  @import url('./../node_modules/css-reset-and-normalize/scss/button-reset.scss');
  @import url('./../node_modules/css-reset-and-normalize/scss/link-reset.scss');

  // Gilroy-Medium font
  @font-face {
    font-family: 'Gilroy-Medium';
    src: url('./assets/fonts/gilroy-medium/gilroy-medium.eot'); /* IE 9 Compatibility Mode */
    src: url('./assets/fonts/gilroy-medium/gilroy-medium.eot?#iefix') format('embedded-opentype'), /* IE < 9 */
      url('./assets/fonts/gilroy-medium/gilroy-medium.woff2') format('woff2'), /* Super Modern Browsers */
      url('./assets/fonts/gilroy-medium/gilroy-medium.woff') format('woff'), /* Firefox >= 3.6, any other modern browser */
      url('./assets/fonts/gilroy-medium/gilroy-medium.ttf') format('truetype'), /* Safari, Android, iOS */
      url('./assets/fonts/gilroy-medium/gilroy-medium.svg#gilroy-medium') format('svg'); /* Chrome < 4, Legacy iOS */
  }

  // Gilroy-Bold font
  @font-face {
    font-family: 'Gilroy-Bold';
    src: url('./assets/fonts/gilroy-bold/gilroy-bold.eot'); /* IE 9 Compatibility Mode */
    src: url('./assets/fonts/gilroy-bold/gilroy-bold.eot?#iefix') format('embedded-opentype'), /* IE < 9 */
      url('./assets/fonts/gilroy-bold/gilroy-bold.woff2') format('woff2'), /* Super Modern Browsers */
      url('./assets/fonts/gilroy-bold/gilroy-bold.woff') format('woff'), /* Firefox >= 3.6, any other modern browser */
      url('./assets/fonts/gilroy-bold/gilroy-bold.ttf') format('truetype'), /* Safari, Android, iOS */
      url('./assets/fonts/gilroy-bold/gilroy-bold.svg#gilroy-bold') format('svg'); /* Chrome < 4, Legacy iOS */
  }
</style>

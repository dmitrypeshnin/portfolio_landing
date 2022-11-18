<template>
    <div class="portfolioBlock">
        <div class="portfolioBlock__inner">
            <h2 class="portfolioBlock__title">Portfolio</h2>
            <div class="portfolioBlock__example">
                <img class="portfolioBlock__img" src="../assets/img/online-fashin-store.jpg" alt="online-fashin-store">
                <h3 class="portfolioBlock__subtitle">Online fashion store - Homepage</h3>
            </div>
            <div class="portfolioBlock__example">
                <img class="portfolioBlock__img" src="../assets/img/reebok_store.jpg" alt="reebok-store">
                <h3 class="portfolioBlock__subtitle">Reebok Store - Concept</h3>
            </div>
            <div class="portfolioBlock__example">
                <img class="portfolioBlock__img" src="../assets/img/braun-landing-page.jpg" alt="">
                <h3 class="portfolioBlock__subtitle">Braun Landing Page - Concept</h3>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "PortfolioBlock"
};
</script>

<style lang="scss" scoped>
    .portfolioBlock {
        background: #F6F6F6;
        padding-top: 112px;
        display: flex;
        flex-direction: column;
        align-items: center;
        &__inner {
            max-width: 936px;
        }
        &__title {
            font-family: 'Gilroy-Bold';
            font-size: 34px;
            line-height: 42px;
            text-align: center;
            color: #070707;
            margin-bottom: 47px;
        }
        &__example {
            margin-bottom: 99px;
        }
        &__img {
            margin-bottom: 45px;
        }
        &__subtitle {
            text-align: center;
            font-family: 'Gilroy-Medium';
            font-size: 18px;
            line-height: 22px;
            text-align: center;
            text-decoration-line: underline;
            color: #070707;
        }
    }
</style>
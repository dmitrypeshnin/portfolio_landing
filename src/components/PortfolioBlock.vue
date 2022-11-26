<template>
    <div class="portfolioBlock">
        <div class="portfolioBlock__inner">
            <h2 class="portfolioBlock__title">Portfolio</h2>
            <div class="portfolioBlock__example" v-for="item in portfolioList" :key="item.name">
                <img class="portfolioBlock__img" :src="item.img" alt="item.name">
                <h3 class="portfolioBlock__subtitle">{{ item.title }}</h3>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "PortfolioBlock",
  data() {
    return {
        portfolioList: [
            {
                name: "online-fashin-store",
                img: require('@/assets/img/online-fashion-store.jpg'),
                title: "Online fashion store - Homepage"
            },
            {
                name: "reebok-store",
                img: require('@/assets/img/reebok-store.jpg'),
                title: "Reebok Store - Concept"
            },
            {
                name: "braun-store",
                img: require('@/assets/img/braun-landing-page.jpg'),
                title: "Braun Landing Page - Concept"
            }
        ]
    }
  }
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
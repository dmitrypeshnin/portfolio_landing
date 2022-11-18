<template>
    <footer class="contactsBlock">
        <h2 class="contactsBlock__title">Contacts</h2>
        <p class="contactsBlock__subtitle">Want to know more or just chat? You are welcome!</p>
        <div class="contactsBlock__button">Send message</div>
        <ul class="contactsBlock__social">
            <li class="contactsBlock__social-icon">
                <a class="contactsBlock_social-link" href="#">
                    <img class="contactsBlock__social-icon" src="../assets/img/linkedin-icon.svg" alt="LinkedIn">
                </a>
            </li>
            <li class="contactsBlock__social-icon">
                <a class="contactsBlock_social-link" href="#">
                    <img class="contactsBlock__social-icon" src="../assets/img/instagram-icon.svg" alt="Instagram">
                </a>
            </li>
            <li class="contactsBlock__social-icon">
                <a class="contactsBlock_social-link" href="#">
                    <img class="contactsBlock__social-icon" src="../assets/img/behance.svg" alt="Behance">
                </a>
            </li>
            <li class="contactsBlock__social-icon">
                <a class="contactsBlock_social-link" href="#">
                    <img class="contactsBlock__social-icon" src="../assets/img/dribble.svg" alt="Behance">
                </a>
            </li>
        </ul>
        <div class="contactsBlock__text">
            Like me on<br>
            LinkedIn, Instagram, Behance, Dribble
        </div>
    </footer>
</template>

<script>
export default {
  name: "ContactsBlock"
};
</script>

<style lang="scss" scoped>
    .contactsBlock {
        padding-top: 111px;
        padding-bottom: 123px;
        display: flex;
        flex-direction: column;
        align-items: center;
        &__title {
            font-family: 'Gilroy-Bold';
            font-size: 34px;
            line-height: 42px;
            color: #070707;
            margin-bottom: 20px;
        }
        &__subtitle {
            max-width: 275px;
            font-family: 'Gilroy-Medium';
            font-size: 18px;
            line-height: 22px;
            text-align: center;
            color: #070707;
            margin: 0 auto;
            margin-bottom: 30px;
        }
        &__button {
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            width: 180px;
            height: 42px;
            border-radius: 50px;
            background: #070707;
            font-family: 'Gilroy-Bold';
            font-size: 18px;
            line-height: 22px;
            text-align: center;
            color: #FFFFFF;
            margin-bottom: 85px;
            cursor: pointer;
            &::after {
                content: '';
                position: absolute;
                width: 166px;
                height: 38px;
                left: 8px;
                top: 10px;
                opacity: 0.1;
                filter: blur(10px);
            }
        }
        &__social {
            max-width: 342px;
            display: flex;
            justify-content: space-between;
            margin-bottom: 45px;
        }
        &__social {
            width: 342px;
        }
        &__text {
            font-family: 'Gilroy-Medium';
            font-size: 14px;
            line-height: 17px;
            text-align: center;
            color: #828282;
        }
    }

</style>
<template>
    <div class="footer footer__bg">
        <div class="container">
            <div class="row">
                <div class="col">
                    <h3 class="footer__title">О нас</h3>
                    <ul class="footer__list footer__list_capitalize footer__list_interval">
                        <li v-for="({ name, path }, i) in footerMenuAboutUs" :key="i">
                            <router-link :to="path" class="footer__link">{{ name }}</router-link>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h3 class="footer__title">Терапия</h3>
                    <ul class="footer__list footer__list_capitalize footer__list_interval">
                        <li v-for="({ name, path }, i) in footerMenuTerapy" :key="i">
                            <router-link :to="path" class="footer__link">{{ name }}</router-link>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h3 class="footer__title">Контакты</h3>
                    <ul class="footer__list footer__list_capitalize">
                        <div class="footer__contact">
                            <img src="../assets/images/icons/phone-icon.svg" class="footerIcons" lt="">
                            <p>+7 (999) 999-99-99</p>
                        </div>
                        <div class="footer__contact">
                            <img src="../assets/images/icons/whatsapp-icon.svg" class="footerIcons" lt="">
                            <p>+7 (999) 999-99-99</p>
                        </div>
                        <div class="footer__contact">
                            <img src="../assets/images/icons/email-icon.svg" class="footerIcons" lt="">
                            <p>dental@mail.ru</p>
                        </div>
                        <div class="footer__contact">
                            <img src="../assets/images/icons/map-icon.png" class="footerIcons" lt="">
                            <p>пр. Проспектовый, 4</p>
                        </div>
                        <div class="footer__contact">
                            <img src="../assets/images/icons/map-icon.png" class="footerIcons" lt="">
                            <p>ул. Уличная, 5</p>
                        </div>

                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { aboutUs } from '../constants/menuLinks'
import { terapy } from '../constants/menuLinks'
export default {
    data() {
        return {
            footerMenuAboutUs: aboutUs,
            footerMenuTerapy: terapy,
        }
    },
}
</script>
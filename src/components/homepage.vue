<template lang="">
<body>
<header>
    <headers/>
    <div class="container">
        <div class="header__img">
            <img class="header__img1" :src="img_header" alt="Kitchen">
        </div>
        <div class="header__Articles__News">
            <p class="header__Articles__News__title"> Articles & News</p>
            <div class="header__Articles__News__link">
                <a class="header__Articles__News__link1" href="#">Home /</a>
                <a class="header__Articles__News__link1" href="#">Blog </a>
            </div>


        </div>
    </div>
</header>
<section class="section center">
    <h2 class="section__header">Latest Post</h2><br>
    <div class="section__block__info">
        <div class="section__img"><img class="section__imgMain" :src="img_Latest_Post" alt=""></div>
        <div class="section__info">
            <h4 class="section__info__header">Low Cost Latest Invented Interior Designing Ideas</h4>
            <p class="section__info__text">Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis
                dignissim maximus.posuere in.Contrary to popular belief.</p>
            <p class="section__info__text">Lorem Ipsum is not simply random text. It has roots in a piece of
                classica.
            </p>
            <div class="section__info__dataInButton">
                <time class="section__info_data"> 26 December,2022 </time>
                <svg width="52" height="53" viewBox="0 0 52 53" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="26" cy="26.5" r="26" fill="#F4F0EC" />
                    <path d="M23.771 33.1855L29.7139 26.4998L23.771 19.8141" stroke="#292F36" stroke-width="2"
                        stroke-linecap="round" stroke-linejoin="round" />
                </svg>
            </div>


        </div>
    </div>



</section>
<section class="section__product center">
    <h1 class="section__product__head">Articles & News</h1>
        <div id="app" class="section__product__wrapper center">
            <div class="section__product__cart" v-for="product in products" :key="product.id">
                <div class="section__product__cart__img">
                    <img class="section__product__cart__img__radiuse" :src="product.imgSrc" alt="foto">
                    <div class="section__product__cart__nameImg">
                        <p class="section__product__cart__nameImg__text">{{ product.category }}</p>
                    </div>
                </div>
                <h3 class="section__product__cart__header">{{ product.title }}</h3>
                <div class="section__product__cart__dataInButton">
                    <time class="section__product__cart__data">{{ product.date }}</time>
                    <svg width="52" height="53" viewBox="0 0 52 53" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <circle cx="26" cy="26.5" r="26" fill="#F4F0EC" />
                        <path d="M23.771 33.1855L29.7139 26.4998L23.771 19.8141" stroke="#292F36" stroke-width="2"
                            stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                </div>
            </div>
        </div>    
        


 


</section>

<footer class="footer center">
    <div class="footer__left">
        <div class="footer__left__logo">
            <div class="footer__left__svg"><svg width="34" height="34" viewBox="0 0 34 34" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M0 34.0003H13.4588V24.499C13.4588 22.4853 15.0898 20.8543 17.1035 20.8543C19.1172 20.8543 20.7482 22.4853 20.7482 24.499V34.0003H33.9975V0C15.2211 0 0 15.2211 0 34.0003Z"
                        fill="#CDA274" />
                </svg></div>
            <div class="header__top__left__text">Interno</div>
        </div>
        <p class="footer__left__text">It is a long established fact that a reader will be distracted lookings.
        </p>
        <div class="footer__left__icons"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16"
                fill="currentColor" class="bi bi-twitter" viewBox="0 0 16 16">
                <path
                    d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z" />
            </svg>
            <p class="footer__left__icons__in"><b>in</b></p>
        </div>



    </div>
    <div class="footer__center">
        <h4 class="footer__center__header">Pages</h4>
        <a class="footer__center__link" href=""><span class="footer__center__link__name">Home</span></a>
        <a class="footer__center__link" href=""><span class="footer__center__link__name">Project</span></a>
        <a class="footer__center__link" href=""><span class="footer__center__link__name">Blog</span></a>

    </div>
    <div class="footer__right">
        <h4 class="footer__right__header">Contact</h4>
        <p class="footer__right__text">55 East Birchwood Ave. Brooklyn, New York 11201 </p>
        <p class="footer__right__text">contact@interno.com
        </p>
        <p class="footer__right__text">+7 (123) 456 - 7890 </p>


    </div>
</footer>
</body>
</template>

<script>
import img_header from '@/assets/img/Images.svg'
import img_Latest_Post from '@/assets/img/Photo.svg'
import product_1 from '@/assets/img_product/product_1.svg'
import product_2 from '@/assets/img_product/product_2.svg'
import product_3 from '@/assets/img_product/product_3.svg'
import product_4 from '@/assets/img_product/product_4.svg'
import product_5 from '@/assets/img_product/product_5.svg'
import product_6 from '@/assets/img_product/product_6.svg'

import footers from './stand/footers.vue'
import headers from './stand/headers.vue'


export default {
    data() {
        return {
            img_header: img_header,
            img_Latest_Post: img_Latest_Post,

            products: [
                {
                    id: 1,
                    imgSrc: product_1,
                    category: 'Kitchen Design',
                    title: 'Let’s Get Solution For Building Construction Work',
                    date: '26 December, 2022',
                },
                {
                    id: 2,
                    imgSrc: product_2,
                    category: 'Living Design',
                    title: 'Low Cost Latest Invented Interior Designing Ideas.',
                    date: '22 December, 2022',
                },
                {
                    id: 3,
                    imgSrc: product_3,
                    category: 'Interior Design',
                    title: 'Best For Any Office & Business Interior Solution',
                    date: '25 December, 2022',
                },
                {
                    id: 4,
                    imgSrc: product_4,
                    category: 'Kitchan Design',
                    title: 'Let’s Get Solution For Building Construction Work',
                    date: '26 December, 2022',
                },
                {
                    id: 5,
                    imgSrc: product_5,
                    category: 'Living Design',
                    title: 'Low Cost Latest Invented Interior Designing Ideas.',
                    date: '22 December, 2022',
                },
                {
                    id: 6,
                    imgSrc: product_6,
                    category: 'Interior Design',
                    title: 'Best For Any Office & Business Interior Solution',
                    date: '25 December, 2022',
                },
                // Добавьте другие статьи, при необходимости
            ]
        };
    },
    components: {
        headers,
        footers

    }
}

</script>
<style lang="scss" scoped>
@import '@/assets/style/_mixsins';
@import '@/assets/style/_vars';
@import '@/assets/style/homepage1';
</style>
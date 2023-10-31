<template lang="">

<headers/>
<div class="container">
    <div class="header__img">
        <img class="header__img1" :src="Photolist4" alt="Kitchen">
    </div>
    <div class="header__Articles__News">
        <p class="header__Articles__News__title"> Our Project</p>
        <div class="header__Articles__News__link">
            <a class="header__Articles__News__link1" href="#">Home /</a>
            <a class="header__Articles__News__link1" href="#">Project </a>
        </div>
    </div>
    <list4/>
</div>



<footers/>

</template>

<script>

import headers from './stand/headers.vue'
import footers from './stand/footers.vue'
import Photolist4 from '@/assets/img/Photolist4.svg'
import list4 from './stand/list4.vue';
export default {
    data() {
        return {
            Photolist4: Photolist4,
        }
    },

    components: {
        headers,
        footers,
        list4

    }


}
</script>
<style lang="scss" scoped>
@import '@/assets/style/_mixsins';
@import '@/assets/style/_vars';


.container {
    position: relative;
    /* Относительное позиционирование для контейнера */
}

.header__Articles__News {
 
    position: absolute;
    display: flex;
    flex-direction: column;
    padding: 41px 78px;
    gap: 10px;
    justify-content: center;
    align-items: center;
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
    background-color: #FFF;
    padding: 20px;
    border: 1px solid #FFF;
    width: 27%;
    /* Настройте процентную ширину текстового блока */
    height: 50%;
    margin: 0 auto;
    /* Центрирует текстовый блок по горизонтали */
    left: 36%;
    bottom: 0;

    /* Отступ снизу равен 0 */
    &__title {
        margin: 0 auto;
        color: #292F36;
        font-family: DM Serif Display;
        font-size: 2.5em;
        font-style: normal;
        font-weight: 400;
        line-height: 125%;
        /* 62.5px */
    }

    &__link1 {
        text-decoration: none;
        color: $ColorText;
        font-family: Jost;
        font-size: 22px;
        font-weight: 400;
        line-height: 150%;
        letter-spacing: 0.22px;

    }
}
</style>
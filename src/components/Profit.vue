<template>
<div class="root">
    <section class="profit">
        <div class="profit__container">
            <h2 class="profit__title">Выгоды</h2>
            <p class="profit__discription">Ваш автомобиль будет блестеть как после покупки, а вы будете довольны выбором</p>
            <div class="profit__list">
                <div class="profit__object">
                    <img src="@/assets/image/profit__location.svg" alt="" class="profit__img">
                    <p class="profit__text">Удобная локация на Ленинградском шоссе
                    </p>
                </div>
                <div class="profit__object">
                    <img src="@/assets/image/profit__money.svg" alt="" class="profit__img">
                    <p class="profit__text">Осмотр автомобиля производится бесплатно</p>
                </div>
                <div class="profit__object">
                    <img src="@/assets/image/profit__payment.svg" alt="" class="profit__img">
                    <p class="profit__text">Для вашего удобства возможен наличный и безналичный расчет</p>
                </div>
                <div class="profit__object">
                    <img src="@/assets/image/profit__achievements.svg" alt="" class="profit__img">
                    <p class="profit__text">Работаем по заказ-наряду с предоставлением гарантийных обязательств</p>
                </div>
                <div class="profit__object">
                    <img src="@/assets/image/profit__fop.svg" alt="" class="profit__img">
                    <p class="profit__text">Для юридических лиц возможна оплата переводом на расчётный счёт </p>
                </div>
            </div>
        </div>
    </section>
</div>

</template>


<script>
export default{
    name: 'MainProfit',
    data(){
        return{
            text: 'asdasdf'
        }
    }
}

</script>


<style scoped lang="scss">

.profit{
    height: 70vh;
    background-image: url(../assets/image/profit-bg.png);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    color: #fff;
    &__container{
        padding: 60px 160px;
    }
    &__title{
        text-align: center;
        font-family: 'roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 54px;
        line-height: 63px;
    }
    &__discription{
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        text-align: center;
        margin-bottom: 60px;
    }
    &__list{
        display: flex;
        justify-content: space-between;
    }
    &__object{
        width: 211px;
        height: 211px;
        background-color: #fff;
        color: #000;
        text-align: center;
        align-items: center;
        border-radius: 5px;
    }
    &__img{
        margin-top: 40px;
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 30px;
    }
    &__text{
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        text-align: center;
        color: #252525;
    }
}

</style>
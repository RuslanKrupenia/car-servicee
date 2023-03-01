<template>
<div class="root">
<section class="services">
    <div class="services__container">
        <h2 class="services__title">Услуги</h2>
        <p class="services__subtitle">Помимо нанесения лакокрасочных покрытий вы можете получить 
            услуги по ремонту и вернуть своей "ласточке" заводской вид</p>
        <div class="services__kinds">
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-detail.png" alt="">
                <p class="services__kind-text">Замена деталей</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-polishing.png" alt="">
                <p class="services__kind-text">Полировка</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-dent.png" alt="">
                <p class="services__kind-text">Исправление вмятин</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-washing.png" alt="">
                <p class="services__kind-text">Чистка(мойка)</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-bumper.png" alt="">
                <p class="services__kind-text">Ремонт бамперов</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-assembly.png" alt="">
                <p class="services__kind-text">Сбор-разбор</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-rent.png" alt="">
                <p class="services__kind-text">Съём</p>
            </div>
            <div class="services__kind">
                <img class="services__kind-img" src="../assets/image/services-painting.png" alt="">
                <p class="services__kind-text">Покраска</p>
            </div>
            <button class="services__button">Подробнее</button>
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
.services{
    max-height: 130vh;
    background-color: #fff;
    &__container{
    padding: 60px 160px 90px;
    }
    &__title{
        font-family: 'roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 54px;
        line-height: 63px;
        text-align: center;
        color: #E7E7E7;
    }
    &__subtitle{
        width: 620px;
        height: 46px;
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        margin-left: auto;
        margin-right: auto;
        text-align: center;
        color: #252525;
        margin-bottom: 60px;
    }
    &__kinds{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
    &__kind{
        width: 265px;
        height: 265px;
        border: 2px solid #D4D4D4;
        margin-bottom: 20px;
        margin-right: 20px;
        text-align: center;
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        color: #252525;
    }
    &__kind-img{
        width: 261px;
        height: 218px;
        margin-bottom: 15px;
    }
    &__king-text{
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        color: #252525;
    }
    &__button{
        width: 170px;
        height: 44px;
        border: 2px solid #D4D4D4;
        margin-right: auto;
        margin-left: auto;
        margin-top: 60px;
    }
}
</style>
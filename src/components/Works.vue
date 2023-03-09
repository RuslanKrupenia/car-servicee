<template>
<div class="root">
    <section class="works">
        <div class="works__container">
            <h2 class="works__title">Примеры работ</h2>
            <p class="works__subtitle">Наша автомастерская - это семейный бизнес, поэтому мы делаем все как для себя. 
                Качественно. Надолго. Без переплат. Посмотрите примеры выполненных работ, 
                чтобы быть уверенным в надежности специалистов, в руки которых вы передадите автомобиль</p>
            <div class="works__examples">
                <div class="works__examples-1"></div>
                <div class="works__examples-2"></div>
                <div class="works__examples-3"></div>
                <div class="works__examples-4"></div>
            </div>
            <div class="works__button">
                <button class="works__more-btn">Посмотреть еще</button>
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
.works{
    min-height: 100vh;
    &__container{
        padding: 60px 160px 90px 160px;
    }
    &__title{
        text-align: center;
        font-family: 'roboto';
        color: #E7E7E7;
        font-style: normal;
        font-weight: 700;
        font-size: 54px;
        line-height: 63px;
    }
    &__subtitle{
        width: 900px;
        height: 69px;
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        margin-left: auto;
        margin-right: auto;
        text-align: center;
        color: #252525;
        margin-top: 10px;
    }
    &__examples{
        display: flex;
        justify-content: space-between;
        margin-top: 60px;
    }
    &__examples-1{
        cursor: pointer;
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-1.png);
        background-position: top center;
        background-size: cover;
        transition: all 1s;
    }
    &__examples-1:hover{
            width: 265px;
            height: 265px;
            background-image: url(@/assets/image/work-before-1.png);
            background-position: top center;
            background-size: cover;
        }

    &__examples-2{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-2.png);
        background-position: top center;
        background-size: cover;
        transition: all 1s;
    }
    &__examples-2:hover{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-before-2.png);
        background-position: top center;
        background-size: cover;
    }
    &__examples-3{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-3.png);
        background-position: top center;
        background-size: cover;
        transition: all 1s;
    }
    &__examples-3:hover{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-before-3.png);
        background-position: top center;
        background-size: cover;
    }
    &__examples-4{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-4.png);
        background-position: top center;
        background-size: cover;
        transition: all 1s;
    }
    &__examples-4:hover{
        width: 265px;
        height: 265px;
        background-image: url(@/assets/image/work-before-4.png);
        background-position: top center;
        background-size: cover;
    }
    &__button{
        text-align: center;
    }
    &__more-btn{
        width: 170px;
        height: 44px;
        border: solid 1px #D4D4D4;
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        color: #252525;
        margin-top: 70px;
        transition: all 1s;
    }
    &__more-btn:hover{
        background-color: #ED7173;
        color: #D4D4D4;
    }
}
</style>
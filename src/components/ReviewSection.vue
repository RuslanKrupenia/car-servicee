<template>
<div class="root">
    <section class="review">
        <div class="review__container">
            <h2 class="review__title">Отзывы клиентов</h2>
            <h3 class="review__subtitle">Посмотрите на отзывы тех, кто уже обращался в нашу автомастерскую</h3>
            <div class="slider">
                <div class="slider__line">
                    <img src="@/assets/image/reviewimg-1.png" alt="" class="slider-img">
                    <img src="@/assets/image/reviewimg-2.png" alt="" class="slider-img">
                    <img src="@/assets/image/reviewimg-3.png" alt="" class="slider-img">
                </div>
                <button class="slider-prev"></button>
                <button class="slider-next"></button>
            </div>
        </div>
    </section>
</div>
</template>

<script>

</script>

<style scoped lang="scss">
.review{
    min-height: 30vh;
    background-image: url(@/assets/image/review-bg.png);
    background-position: top center;
    background-repeat: no-repeat;
    background-size: cover;
    &__container{
        padding: 62px 215px 90px;
    }
    &__title{
        font-family: 'roboto';
        font-style: normal;
        font-weight: 700;
        font-size: 54px;
        line-height: 63px;
        text-align: center;
        color: #FFFFFF;
    }
    &__subtitle{
        font-family: 'arial';
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        text-align: center;
        color: #FFFFFF;
        margin-top: 10px;
        margin-bottom: 66px;
    }

}

</style>
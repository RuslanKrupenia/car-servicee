<template>
<div class="root">
<section class="about">
    <div class="about__container">
    <h2 class="about__title">Подробнее о Центре Автопокраски</h2>
    <p class="about__subtitle">Полное или частичное восстановление ЛКП за короткие сроки и с гарантией качества</p>
        <div class="about__information">
            <div class="about__info-1">
                <p class="about__info-text">Уже 6 лет мы занимаемся качественным 
                    восстановлением машин от повреждений разной сложности. Рейтинг нашей мастерской на Яндексе составляет 4,5.</p>
            </div>
            <div class="about__info-2">
                <p class="about__info-text">Заметили следы естественного износа? 
                    Мы легко удалим царапины, вмятины, коррозию и ржавчину, которые могут изрядно подпортить внешний вид автомобиля. 
                    </p>
            </div>
            <div class="about__info-3">
                <p class="about__info-text">Попали в ДТП и хотите сохранить вид вашего авто? Исправим повреждения 
                    за короткий срок!</p>
            </div>
            <div class="about__info-4">
                <p class="about__info-text">Использование качественных материалов: Sikkens, Akzo, Nobel, Brulex, 3M, Car System, Body Reoflex, позволяет сохранить результат работы надолго. Гарантия на все виды работ составляет 1 год.</p>
            </div>
        </div>
    </div>
</section>
</div>
</template>




<script>
export default{
    name: 'MainAbout',
    data(){
        return{
            text: 'asdasdf'
        }
    }
}
</script>




<style scoped lang="scss">
.about{
    height: 90vh;
    width: 100%;
    background-color: #fff;
    &__container{
        padding: 58px 268px 29px 255px;
    }
    &__title{
        width: 900px;
        height: 36px;
        font-weight: 700;
        font-size: 54px;
        line-height: 63px;
        margin-left: auto;
        margin-right: auto;
        color: #E7E7E7;
        margin-bottom: 30px;
        font-family: 'roboto';
    }
    &__subtitle{
        font-family: 'arial';
        width: 800px;
        height: 23px;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        margin-left: auto;
        margin-right: auto;
    }
    &__information{
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        flex-wrap: wrap;
        margin-top: 20px;
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        font-family: 'arial';
    }
    &__info-1{
        width: 435px;
        height: 160px;
        background-image: url(@/assets/image/about-bg-1.svg);
        background-repeat: no-repeat;
        padding-top: 50px;
        padding-left: 30px;
    } 
    &__info-2{
        width: 435px;
        height: 210px;
        background-image: url(@/assets/image/about-bg-2.svg);
        background-repeat: no-repeat;
        padding-top: 50px;
        padding-left: 30px;
    } 
    &__info-3{
        width: 435px;
        height: 139px;
        background-image: url(@/assets/image/about-bg-3.svg);
        background-repeat: no-repeat;
        padding-top: 50px;
        padding-left: 30px;
    } 
    &__info-4{
        width: 435px;
        height: 185px;
        background-image: url(@/assets/image/about-bg-4.svg);
        background-repeat: no-repeat;
        padding-top: 50px;
        padding-left: 30px;
    } 
}
</style>
<template>
<div class="root">
<section class="header">
    <div class="header__container">
        <div class="header__menu">
            <div class="header__logo">
                <img src="@/assets/image/header-logo.svg" alt="" class="logo-img">
            </div>
            <div class="header__navigation">
                <ul class="navigation__menu">
                    <li class="navigation__item"><a href="#" class="navigation__link">Главная</a></li>
                    <li class="navigation__item"><a href="#services" class="navigation__link">Услуги</a></li>
                    <li class="navigation__item"><a href="#" class="navigation__link">Примеры работ</a></li>
                    <li class="navigation__item"><a href="#" class="navigation__link">Контакты</a></li>
                </ul>
            </div>
            <div class="header__location"><a href="https://www.google.com.ua/maps/place/%D1%83%D0%BB.+%D0%9A%D1%80%D0%B5%D1%89%D0%B0%D1%82%D0%B8%D0%BA,+25,+%D0%9A%D0%B8%D0%B5%D0%B2,+02000/@50.4444625,30.5205899,17z/data=!3m1!4b1!4m6!3m5!1s0x40d4ce55d0276e59:0xb03fd0a90c6de69a!8m2!3d50.4444625!4d30.5227786!16s%2Fg%2F11c26xs9sn?hl=ru" class="location-link">Киев, улица Крещатик 25(1)</a></div>
            <div class="header__number"><a href="tel:380500368958" class="number-link">+380 (50) 668 8878</a></div>
        </div>
        <hr>
        <div class="header__info">
            <h2 class="header__name">Кузовной ремонт любой сложности</h2>
            <h3 class="header__name-location">на Крещатике в Киеве</h3>
            <div class="header__buttons">
                <button class="header__btn-form">Оставить заявку</button>
                <button class="header__btn-foto">Оценить стоимоть ремонта по фото</button>
            </div>
            <p class="header__promotion">Оставляйте заявку сейчас и получите <span class="header__span">10 % скидку</span> на покраску</p>
        </div>
            <div class="header__achievements">
                <div class="achivements__info">
                    <img src="@/assets/image/chievements-img-1.svg" alt="" class="achievements-img">
                    <p class="info__text">Гарантия 1 год</p>
                </div>
                <div class="achivements__info">
                    <img src="@/assets/image/chievements-img-2.svg" alt="" class="achievements-img">
                    <p class="info__text">Делаем как для себя: 
                        качественно и без переплат</p>
                </div>
                <div class="achivements__info">
                    <img src="@/assets/image/chievements-img-3.svg" alt="" class="achievements-img">
                    <p class="info__text">Салон расположен 
                        в пределах центра Киева </p>
                </div>
            </div>
    </div>
</section>
</div>
</template>



<script>
export default{
    name: 'MainHeader',
    data(){
        return{
            text: 'asdasdf'
        }
    }
}

</script>


<style scoped lang="scss">

.header{
    font-family: 'roboto';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
    &__container{
        background-image: url(@/assets/image/header-bg.png);
        background-size: cover;
        background-position: top center;
        background-repeat: no-repeat;
        height: 130vh;
        width: 100%;
    }
    &__menu{
        display: flex;
        justify-content: space-between;
        padding-left: 40px;
        padding-right: 40px;
    }
    
    &__navigation, &__location, &__number{
        padding-top: 50px;
        padding-bottom: 20px;
    }
    &__logo{
        width: 187px;
        height: 71px;
        padding-top: 16px;
        padding-bottom: 5px;
    }
    &__info{
        color: #fff;
    }
    &__name{
        width: 410px;
        height: 112px;
        font-weight: 400;
        font-size: 48px;
        line-height: 56px;
        margin-bottom: 17px;
    }
    &__name-location{
        width: 470px;
        height: 33px;
        font-style: normal;
        font-weight: 400;
        font-size: 28px;
        line-height: 33px;
        margin-bottom: 50px;
    }
    &__btn-form{
        color: #fff;
        width: 170px;
        height: 44px;
        border: solid 1px #fff;
        margin-right: 0px;
        font-family: 'arial';
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        margin-right: 20px;
    }
    &__btn-foto{
        color: #fff;
        width: 304px;
        height: 44px;
        border: solid 1px #fff;
        font-family: 'arial';
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
    }
    &__promotion{
        font-family: 'arial';
        font-weight: 400;
        font-size: 16px;
        line-height: 18px;
        width: 469px;
        height: 18px;
    }
    &__span{
        color: #ED7173;
    }
    &__info{
        padding: 180px 690px 150px 255px;
    }
    &__buttons{
        display: flex;
        margin-bottom: 20px;
    }
    &__achievements{
        font-family: 'arial';
        color: #fff;
        text-align: center;
        padding: 0px 180px 65px 180px;
        margin-bottom: 65px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-weight: 400;
        font-size: 18px;
        line-height: 21px;
    }
}
.achivements__info{
    width: 276px;
    height: 120px;
    text-align: center;
    border: 1px solid #fff;
    

}
.achievements-img{
    margin-right: auto;
    margin-left: auto;
    margin-top: 5%;
    margin-bottom: 14px;
}
a{
    color: #fff;
}
.logo-img{

    width: 187px;
    height: 71px;
}
.navigation__menu{
    display: flex;
    justify-content: space-between;
    width: 404px;
    height: 20px;
    &__item{
        transition: all 0.5s;
    }

}
    li:hover{
        border-bottom: 1px solid #fff;
    }

</style>
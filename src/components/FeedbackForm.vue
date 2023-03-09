<template>
<div class="root">
<section class="feedback">
    <div class="feedback__container">
        <h2 class="feedback__title">Испытайте снова ту радость, когда вы только купили блестящую 
            машинку в салоне! Качественный покрас и ремонт автомобиля 
            - это отличный вариант обновить авто без покупки нового</h2>
            <div class="feedback__cont">
              <form class="feedback__form"  @submit.prevent="submitForm" enctype="multipart/form-data">
                <div class="feedback__add">
                  <p class="feedback__add-text">Вы можете добавить фото для оценки стоимости ремонта через форму</p>
                  <input  class="feedback__add-file"  type="file" id="file" accept="image/png, image/jpeg" @change="onFileChange">
                </div>
                <div class="feedback__form-info">
                  <input  class="feedback__input" placeholder="Ваше имя" type="text" id="name" v-model="name" required>
                  <input  class="feedback__input" placeholder="Номер телефона" type="tel" id="phone" v-model="phone" required>
                  <button class="feedback__send-btn" type="submit">Отправить</button>
                </div>
              </form>
            </div>
            </div>
</section>
</div>
</template>

<script>
import axios from 'axios';
import Swal from 'sweetalert2';

export default {
  data() {
    return {
      name: '',
      phone: '',
      file: null,
      telegramBotToken: '6022029255:AAHnMDCeSYPYlO6dLzmruO5M06ugwCsVEqM',
      chatId: '-807488960'
    };
  },
  methods: {
    onFileChange(event) {
      this.file = event.target.files[0];
    },
    submitForm() {
      const formData = new FormData();
      formData.append('document', this.file);
      formData.append('chat_id', this.chatId);
      formData.append('caption', `
        Новая заявка на обратный звонок:
        Имя: ${this.name}
        Номер телефона: ${this.phone}
      `);

      const telegramUrl = `https://api.telegram.org/bot${this.telegramBotToken}/sendDocument`;

      axios.post(telegramUrl, formData)
        .then(response => {
          console.log(response);
          if (response.data.ok === true) {
            Swal.fire (
              'Дякую!',
              'Повідомлення успішно надіслано 🎉',
            )
          }
        })
        .catch(error => {
          console.error('Произошла ошибка при отправке сообщения в Telegram:', error);
          // Здесь можно добавить код для обработки ошибки отправки формы
        });
    }
  }
}
</script>

<style scoped lang="scss">
.feedback{
  min-height: 70vh;
  background-image: url(@/assets/image/feedback-bg.png);
  background-size: cover;
  background-position: center center;
  &__container{
    padding: 80px 285px 90px;
  }
  &__title{
    font-family: 'roboto';
    font-style: normal;
    font-weight: 400;
    font-size: 28px;
    line-height: 33px;
    text-align: center;
    color: #FFFFFF;
  }
  &__cont{
    width: 740px;
    height: 172px;
    margin-left: auto;
    margin-right: auto;
  }
  &__form{
    display: flex;
    justify-content: space-between;
  }
  &__add{
    width: 286px;
    height: 112px;
    margin-top: 62px;
  }
  &__add-text{
    font-family: 'arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
    color: #FFFFFF;
    margin-bottom: 32px;
  }
  &__add-file{
    width: 170px;
    height: 45px;
  }
  &__form-info{
    margin-top: 60px;
    margin-left: 95px;
  }
  &__input{
    display: flex;
    width: 360px;
    height: 45px;
    margin-bottom: 20px;
    border: 2px solid #fff;
    color: #000;
    border-radius: 4px;
    padding-left: 17px;
    font-family: 'arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
  }
  input::placeholder {
    color: #D4D4D4; 
    font-family: 'arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
  }
  &__send-btn{
    text-align: center;
    width: 360px;
    height: 44px;
    border: 2px solid #fff;
    border-radius: 4px;
    font-family: 'arial';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
    color: #FFFFFF;
    background-color: none;
  }
}

</style>
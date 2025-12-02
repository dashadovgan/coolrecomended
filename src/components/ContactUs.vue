<template>
  <section class="contact-wrapper">
    <div class="contact-container">

      <!-- Горизонтальна лінія зверху -->
      <div class="line-horizontal"></div>

      <!-- Заголовок -->
      <h2 class="contact-title center">Контактна інформація</h2>

      <!-- Горизонтальна лінія знизу -->
      <div class="line-horizontal"></div>

      <!-- Основний текст -->
      <p class="contact-text center">
        Класно, що хочеш дізнатись більше.<br>
        Зв’яжись із тими, хто вірить у людей.
      </p>

      <!-- Контактні особи -->
      <div class="contacts-block">
        <div class="contact-item">
          <span class="contact-name">Оксана Медведєва</span>
          <span class="contact-phone">+380965450043</span>
        </div>
        <div class="contact-item">
          <span class="contact-name">Євген Дігтяренко</span>
          <span class="contact-phone">+380964642615</span>
        </div>
        <div class="contact-item">
          <span class="contact-name">Ілля Москаленко</span>
          <span class="contact-phone">+380685543529</span>
        </div>
        <div class="contact-item">
          <span class="contact-name">Юлія Нечипорук</span>
          <span class="contact-phone">+380678719154</span>
        </div>
        <div class="contact-item">
          <span class="contact-name">Напиши нам</span>
          <span class="contact-phone">med28061968@uk.net</span>
        </div>
      </div>

      <!-- Соцмережі -->
      <div class="social-block">
        <a href="https://www.instagram.com/n21ua?igsh=Z3VqdnVhZG51aHNm" target="_blank">Instagram</a>
        <a href="https://t.me/network21ua" target="_blank">Telegram</a>
        <a href="https://www.facebook.com/share/16SBehCSdb/" target="_blank">Facebook</a>
        <a href="https://www.n21corp.com/overview.aspx" target="_blank">Офіційний сайт</a>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: "ContactInfo"
};
</script>

<style scoped>
.contact-wrapper {
  background-color: #15232C;
  padding: 0;
  display: flex;
  justify-content: center;
  width: 100%;
}

.contact-container {
  width: 95%;
  max-width: 1000px;
}

/* Горизонтальні лінії */
.line-horizontal {
  width: 100%;
  height: 3px;
  background-color: #3D4D55;
  margin: 20px auto;
  border-radius: 2px;
}

/* Заголовок */
.contact-title {
  font-size: 2.4rem;
  color: white;
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  text-align: center;
  margin-bottom: 25px;
}

/* Основний текст */
.contact-text {
  color: #e6e6e6;
  font-size: 1.2rem;
  line-height: 1.7;
  margin-bottom: 35px;
  font-family: 'Playfair Display', serif;
  text-align: center;
}

/* Контакти */
.contacts-block {
  display: flex;
  flex-direction: column;
  gap: 14px;
  margin-bottom: 30px;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.contact-item {
  color: #e6e6e6;
  font-size: 1.15rem;
  font-family: 'Playfair Display', serif;
  padding: 10px 15px;
  border-left: 4px solid #B58863;
  background-color: #3D4D55;
  border-radius: 8px;
  display: flex;
  justify-content: space-between;
  width: 400px; /* фиксированная ширина */
}

.contact-name {
  display: inline-block;
  width: 180px; /* одинаковая ширина для всех имен */
}

.contact-phone {
  display: inline-block;
  text-align: right;
  width: 200px; /* одинаковая ширина для номеров */
}

/* Соцмережі */
.social-block {
  display: flex;
  gap: 18px;
  flex-wrap: wrap;
  justify-content: center;
}

.social-block a {
  color: #B58863;
  font-size: 1.1rem;
  font-family: 'Playfair Display', serif;
  text-decoration: none;
  padding: 8px 14px;
  border: 2px solid #B58863;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.social-block a:hover {
  background-color: #B58863;
  color: #15232C;
}

@media (max-width: 500px) {
  .contact-item {
    flex-direction: column;       /* имя сверху, номер снизу */
    width: 280px;                 /* фиксированная, но не 100% */
    align-items: center;           /* выравнивание содержимого по центру */
    justify-content: center;
    margin: 0 auto;                /* центрирование самого блока */
  }
  .contact-name,
  .contact-phone {
    width: auto;                  /* текст не ограничен фикс. шириной */
    text-align: center;           /* текст по центру блока */
    display: block;
  }
  .contacts-block {
    align-items: center;           /* блоки по центру */
  }
}

</style>

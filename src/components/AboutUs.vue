<template>
  <section class="about-wrapper">

    <!-- Верхний блок с текстом и первой галереей -->
    <div class="about-container">
      <div class="about-title-wrapper">
  <h1 class="about-title">Про нас</h1>
</div>


      <div class="about-text">
        <p class="striped">
          Наш бізнес-клуб «Класно..... Рекомендую!!!» вже 10 років зростає в міжнародній освітній екосистемі
          <a href="https://network21.com" target="_blank" class="link-highlight">Network TwentyOne</a> — одній із найпотужніших систем підтримки підприємців у світі.
          Джим і Ненсі Дорнан — засновники світового руху Network 21, що більше 30 років допомагає людям будувати бізнес, розвивати навички та створювати успішні спільноти.
        </p>

        <div class="mini-gallery">
          <div class="mini-photo frame-light">
            <img src="@/assets/photo_Nancy.jpg" alt="Ненсі Дорнан">
            <div class="mini-caption">
  <p>Джим і Ненсі Дорнан — засновники Network TwentyOne</p>
  <p>Джим і Ненсі створили міжнародну спільноту Лідерів та підприємців, засновану на любові, взаємоповазі, прихильності та позитивному ставленні одне до одного.</p>
</div>
 </div>
          <div class="mini-photo frame-light">
            <img src="@/assets/photo_Oxana.jpg" alt="Оксана Медведева">
            <div class="mini-caption">
            <p>Незалежні підприємці, Активні партнери бізнес школи Нетворк 21, засновники бізнес-клубу "Класно..... Рекомендую!!!</p>
            </div>
        
          </div>
        </div>

        <p class="striped">
          За ці роки ми відвідали десятки міжнародних семінарів, де вчилися у топових світових спікерів: Джим і Ненсі Дорнан, 
          Кіт Абрахам, Джон Максвелл, Ханс і Єва Нусхольд, Іренке Немет, Пітер Метц, Майкл Вілсон, Скіп Рос, Массімо Біні.
          Це лідери, які формують мислення, культуру бізнесу і задають стандарти розвитку на роки вперед.
        </p>
      </div>
    </div>

    <!-- Вся галерея на всю ширину с подписью -->
    <div class="full-width-gallery">
      <div class="mini-gallery2">
  <div class="gallery-title">
    <span class="bigger">Ці фото</span>
    <span>— про наш шлях</span>
    <span>і нашу силу</span>
  </div>

  <div class="mini-photo">
    <img src="@/assets/photo_Abroad1.jpg" alt="">
  </div>

  <!-- Второе фото заменяем на видео -->
<div class="mini-photo">
  <video autoplay muted loop playsinline width="100%" height="400">
    <source src="/videos/video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

  <div class="mini-photo">
    <img src="@/assets/photo_Abroad3.jpg" alt="">
  </div>
  <p class="captionGallery2">Кожна подія від Нетворк 21 - це завжди особистий План зростання, бачення Великих Можливостей, Ключ до свого внутрішнього "Я"

Кожна подія від Нетворк 21 - це ПРО "Мати настрій...і хочу..і можу", доступ до інтелектуальної власності міжнародних Практиків Вільного підприємництва з 6 континентів</p>

</div>

    </div>
    <!-- Нижний блок с текстом и преимуществами -->
    <div class="about-container">
      


<div class="about-title-wrapper">
  <h2 class="about-title center">Що нам дає Network 21</h2>
</div>


      <ul class="benefits">
        <li>Глобальний масштаб: присутність у 40+ країнах</li>
        <li>Сотні бізнес-подій щотижня, найбільша освітня екосистема в індустрії</li>
        <li>N21Mobile — доступ до преміального навчання 24/7</li>
        <li>Лідери світового класу, у яких ми навчаємося особисто</li>
        <li>Ком’юніті, що мислить на рівні міжнародних стандартів</li>
      </ul>

      <p class="striped">
        Ми відкриваємо двері для тих, хто хоче: рости в сильному оточенні; отримувати знання від світових лідерів; 
        будувати власний бізнес із міжнародною підтримкою; запускати стартапи, які мають фундамент, структуру та правильне мислення; 
        відчути драйв команди, яка рухається вперед. Це середовище — для тих, хто готовий грати на рівні вище. Якщо це про тебе — приєднуйся.
      </p>
    </div>

  </section>
</template>


<style scoped>
.about-wrapper {
  width: 100%;
  background-color: #15232C
}

.about-container {
  width: 90%;
  max-width: 1100px;
  margin: 0 auto;
  padding: 20px 0;
}

.about-title {
  font-size: 3rem;
  text-align: center;
  color: white;
  margin-bottom: 40px;
  font-family: 'Playfair Display', serif;
}

.striped {
  position: relative;
  padding-left: 25px;
  background-color: #2e3f49;
  border-radius: 10px;
  margin-bottom: 22px;
  font-size: 1.3rem;
  line-height: 1.7;
  color: white;
  font-family: 'Playfair Display', serif;
}

.striped::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 6px;
  height: 100%;
  background-color: #B58863;
  border-radius: 3px;
}

.link-highlight {
  color: #B58863;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s ease;
}

.link-highlight:hover {
  color: #15232C;
  text-decoration: underline;
}




.gallery-title {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: white;
  font-weight: 700;
  margin-bottom: 20px;
  font-family: 'Playfair Display', serif;
  text-transform: uppercase;
  text-align: center;
}

.gallery-title span {
  display: block;
  line-height: 1.2;
}

/* Огромный первый уровень */
.gallery-title .bigger {
  font-size: 60px !important;
}

/* Второй уровень */
.gallery-title span:nth-child(2) {
  font-size: 30px;
}

/* Третий уровень */
.gallery-title span:nth-child(3) {
  font-size: 40px;
}

/* Первая мини-галерея */
.mini-gallery {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 22px;
  margin: 30px 0 40px;
}

.frame-light {
  padding: 12px;
  background-color: #223642;
  border-radius: 14px;
}

.mini-photo img {
  width: 100%;
  border-radius: 14px;
  object-fit: cover;
  box-shadow: 0 6px 14px rgba(0,0,0,0.15);
}

.mini-caption {
  font-size: 18px;
  color: white;
  text-align: center;
  margin-top: 8px;
  font-family: 'Playfair Display', serif;
}

/* Вторая мини-галерея на всю ширину */
.full-width-gallery {
  width: 100%;
  background-color: #15232C;
  padding: 40px 0;
  display: flex;
  justify-content: center;
}

.mini-gallery2 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  width: 95%;
  max-width: 1200px;
  padding: 20px;
  border-radius: 14px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.25);
  background-color: #3D4D55;
}

.mini-gallery2 .mini-photo {
  border: 4px solid white; /* рамка */
  border-radius: 14px;
  overflow: hidden;
  padding: 0;
  height: 400px; /* фиксированная высота всех медиа */
  background-color: transparent;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: transform 0.3s ease; 
}

.mini-gallery2 .mini-photo img,
.mini-gallery2 .mini-photo video {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 0; /* убираем радиус у медиаконтента */
  display: block;
  transition: transform 0.5s ease, box-shadow 0.5s ease; 
}



.mini-gallery2 .mini-photo img:hover {
  transform: scale(1.05);
  box-shadow: 0 10px 20px rgba(0,0,0,0.25);
}

.mini-gallery2 .mini-photo:nth-child(3) {
  grid-column: 1 / -1;
  width: 80%;
  justify-self: center;
}


.mini-gallery2 .mini-photo video:hover {
  transform: scale(1.05);
  box-shadow: 0 10px 20px rgba(0,0,0,0.25);
}
.captionGallery2{
    position: relative;
  padding-left: 25px;
  border-radius: 10px;
  margin-bottom: 22px;
  padding-top: 70px;
  font-size: 1.3rem;
  line-height: 1.7;
  color: white;
  font-family: 'Playfair Display', serif;
}
.benefits {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 22px 28px;
  padding: 0;
  margin: 40px 0;
  list-style: none;
}

.benefits li {
  background-color: white;
  color: #15232C;
  padding: 18px 20px;
  width: 260px;
  border-radius: 14px;
  font-size: 1.2rem;
  font-family: 'Playfair Display', serif;
  line-height: 1.5;
  display: flex;
  align-items: center;
  gap: 12px;
  box-shadow: 0 6px 14px rgba(0,0,0,0.15);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
   border: 4px solid #3D4D55;
}

.benefits li:hover {
  transform: translateY(-6px);
  box-shadow: 0 10px 22px rgba(0,0,0,0.25);
}

.benefits li::before {
  content: "~";
  font-size: 1.4rem;
  flex-shrink: 0;
 
}
.about-title-wrapper {
  position: relative;
  width: 100%;
  margin: 40px 0;
}

.about-title-wrapper::before,
.about-title-wrapper::after {
  content: "";
  position: absolute;
  left: 0;
  width: 100%;
  height: 3px; /* толщина полосы */
  background-color: #3D4D55; /* светло-синий */
}

.about-title-wrapper::before {
  top: 0;
}

.about-title-wrapper::after {
  bottom: 0;
}

.about-title {
  font-size: 3rem;
  text-align: center;
  color: white;
  font-family: 'Playfair Display', serif;
  padding: 20px 0; /* чтобы текст не прилипал к линиям */
  margin: 0; /* убираем внешний margin */
}

@media (max-width: 700px) {
  .mini-gallery {
    grid-template-columns: 1fr;
  }
  .about-title {
    font-size: 2.4rem;
  }
  .mini-gallery2 {
    grid-template-columns: 1fr;
    padding: 40px;
    
  }
  .mini-gallery2 .mini-photo{
    margin-bottom: 30px;
  }
  .mini-gallery2 .mini-photo:nth-child(3) {
    width: 100%;
  }
  .gallery-title span {
    font-size: 2rem;
  }
  .captionGallery2{
    padding-top: 0;
  }
}
</style>

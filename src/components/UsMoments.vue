<template>
  <section class="meetings-wrapper">
    <div class="meetings-container">

      <!-- Горизонтальна лінія зверху -->
      <div class="line-horizontal"></div>

      <!-- Заголовок -->
      <h2 class="about-subtitle center">Наш довсвід</h2>

      <!-- Горизонтальна лінія знизу -->
      <div class="line-horizontal"></div>

      <!-- Блок історій + вертикальна лінія -->
      <div class="stories-block">
       
 <div class="story-item">
  <div class="story-photo-wrapper">
    <img src="@/assets/photoMikeWilson.jpg" alt="Майк Вілсон" class="story-photo" />
  </div>
  <p class="story-text">
    <strong>Майк Вілсон</strong> — професійний тенісист, який виступав на міжнародних змаганнях 
    та працював тренером у клубах Південної Каліфорнії.  
    «Навіть із 25–30 доларами на годину ми розуміли, що такими темпами ніколи не станемо вільними. 
    Було складно уявити, як ми заведемо сім’ю».
  </p>
</div>

        <p class="story-text">
          Коли Майк познайомився з бізнесом, його тренування були розписані з 7 ранку до 10 вечора.  
          На запитання «Чого ти хочеш від цього бізнесу?» він відповів: «Усього».  
          «Коли тобі це потрібно?» — «Учора».
        </p>

        <p class="story-text">
          «Ми з дружиною зрозуміли, що якщо цей бізнес почне працювати, 
          він дасть нам фінансові можливості, про які ми мріяли, і час, якого бракувало. 
          Тоді ми ще не усвідомлювали, наскільки сильно ми його полюбимо».
        </p>
<div class="story-item">
  <div class="story-photo-wrapper">
    <img src="@/assets/photoSkipRoss.jpg" alt="Майк Вілсон" class="story-photo" />
  </div>
        <p class="story-text">
          <strong>Скіп Росс</strong> — приклад потужної сімейної спадковості в бізнесі Network 21. 
          Сьогодні їхній сімейний бізнес простягається по всій земній кулі. 
          Маленькі рішення сім’ї Скіпа вплинули на життя сотень тисяч людей.  
          Друге й третє покоління — Мелоді та Кріс Фаррелл, Стівен і Дженні Росс — 
          активно продовжують розвивати спільну справу.
        </p>
</div>
<div class="story-item">
  <div class="story-photo-wrapper">
    <img src="@/assets/photoDeviddornan.jpg" alt="Майк Вілсон" class="story-photo" />
  </div>
        <p class="story-text">
          <strong>Девід Дорнан</strong> родом із Каліфорнії. Закінчив Лібертійський університет, 
          отримавши ступінь у галузі теології та фінансів.  
          Розпочав кар’єру у сфері комерційної нерухомості в Атланті, де й живе сьогодні.
        </p>
</div>
        <p class="story-text">
          Девід потрапив до статті «Неймовірні підприємці» на Forbes.com, 
          де було представлено успішних лідерів бізнесу.  
          Як син засновників Network TwentyOne, Джима та Ненсі Дорнан, він ріс, 
          спостерігаючи за бізнесом зсередини, і досягнув власного вражаючого успіху.
        </p>
      </div>

      <!-- Відео -->
    <div class="video-gallery">
  <div class="video-item">
    <video 
      src="/videos/video3.mp4"
      controls
      autoplay
      muted
      playsinline
      loop
    ></video>
  </div>
</div>


      
    </div>
  </section>
</template>



<style scoped>
/* Фон всього блоку */
.story-item {
  display: flex;
  flex-direction: column; /* фото сверху, текст снизу */
  align-items: center;    /* центрируем фото */
  margin-bottom: 40px;
}

.story-photo-wrapper {
  width: 220px;
  height: 220px;
  border: 2px solid #ffffff; /* тонкая рамка */
  border-radius: 50%;         /* круглая */
  overflow: hidden;           /* обрезаем края */
  margin-bottom: 20px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.story-photo-wrapper:hover {
  transform: scale(1.08);      /* легкое приближение */
  box-shadow: 0 8px 20px rgba(0,0,0,0.35);
}

.story-photo {
  width: 100%;
  height: 100%;
  object-fit: cover; /* сохраняем пропорции */
}

.story-text {
  font-size: 1.22rem;
  line-height: 1.75;
  color: #e6e6e6;
  font-family: 'Playfair Display', serif;
  text-align: center; /* текст по центру */
}


.meetings-wrapper { 
  width: 100%; 
  padding: 30px 20px; 
  background-color: #15232C; 
  display: flex; 
  justify-content: center; 
}

.meetings-container { 
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
.about-subtitle { 
  font-size: 2.4rem; 
  color: white; 
  font-weight: 700; 
  font-family: 'Playfair Display', serif; 
  letter-spacing: 1px;
  text-align: center;
}

/* ВЕРТИКАЛЬНА ЛІНІЯ ДЛЯ ВСЬОГО ТЕКСТОВОГО БЛОКУ */
.stories-block {
  background-color: #3D4D55;
  padding: 25px 30px 25px 40px;
  border-left: 4px solid #B58863;
  margin-bottom: 50px;
  border-radius: 10px;
}

/* Параграфи */
.story-text {
  font-size: 1.22rem;
  line-height: 1.75;
  color: #e6e6e6;
  margin-bottom: 18px;
  font-family: 'Playfair Display', serif;
}

.story-text strong {
  color: #B58863;
}

/* Відео */
.video-gallery { 
  display: flex; 
  justify-content: center; 
  margin-top: 30px;
}

.video-item video { 
  width: 900px;            /* 🔥 фіксована ширина */
  height: 506px;           /* 🔥 фіксована висота (16:9) */
  max-width: 100%;         /* адаптація під мобільні */
  object-fit: cover;       /* відео рівно обрізається і не сплющується */
  border-radius: 14px; 
  background: #3D4D55;
  box-shadow: 0 12px 32px rgba(0,0,0,0.45); 
  transition: transform 0.45s ease, box-shadow 0.45s ease; 
}



/* Ховер ефект */
.video-item video:hover { 
  transform: scale(1.03); 
  box-shadow: 0 20px 50px rgba(0,0,0,0.65); 
}
.title {
  font-size: 1.22rem;
  line-height: 1.75;
  color: #e6e6e6;
  margin: 18px auto 0;
  font-family: 'Playfair Display', serif;
  text-align: center;   
  max-width: 900px;       
}

@media (max-width: 700px) {
  .about-subtitle { font-size: 1.9rem; }
  .story-text { font-size: 1.07rem; }
  .stories-block { padding-left: 20px; padding-right: 20px; }
}
</style>

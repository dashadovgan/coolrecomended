<template>
  <section class="join-wrapper">
    <div class="join-container">

      <!-- ВЕРХНЯ ЛІНІЯ -->
      <div class="line-horizontal"></div>

      <h2 class="block-title">Як до нас долучитися</h2>

      <!-- НИЖНЯ ЛІНІЯ -->
      <div class="line-horizontal"></div>


      <!-- КРОКИ -->
      <div class="steps-block">

        <div class="step">
          <h3 class="step-title">1️⃣ Знайомство</h3>
          <p class="step-text">
           Ви потрапляєте на зустріч Клубу «Класно… Рекомендую».
Тут панує атмосфера легкості, щирості та взаємної підтримки.</p>

<p class="step-text">Це не лекція і не презентація — це теплий простір, де можна вільно поспілкуватися, познайомитися з однодумцями та відчути енергію людей, які розвиваються.
Ви з першої хвилини бачите: тут немає тиску, поспіху чи продажів — тільки природна комунікація, відкритість та реальні історії учасників.</p>

<p class="step-text">Знайомство створене так, щоб ви могли розслабитися, відкласти щоденні турботи та переключитися на нові ідеї, які надихають.</p>
       
        </div>

        <div class="step">
  <h3 class="step-title">2️⃣ Ідеї та натхнення</h3>

  <p class="step-text">
    Через ігропрактику, дебати, командні завдання чи формат Real Talk  
    ви бачите, як працює розвиток через комунікацію. Тут кожен формат створений  
    не просто «для розваги», а щоб м’яко, природно включити вас у процес навчання.
  </p>

  <p class="step-text">
    Ви відчуваєте, як через обговорення й живі взаємодії відкриваються нові думки,  
    з’являються ідеї та приходить натхнення. Люди діляться своїми історіями,  
    досвідом, помилками і перемогами — і це заряджає більше, ніж будь-яка лекція.
  </p>

</div>


        <div class="step">
          <h3 class="step-title">3️⃣ Наступний крок — N21 Mobile</h3>
          <p class="step-text">
            Якщо вам відгукується підхід, ви можете пройти тест-драйв  
            мобільного додатку і побачити систему розвитку зсередини.  
            Також ви дізнаєтесь про можливість створення власного бізнесу  
            в партнерстві з міжнародною компанією з перевіреною системою підтримки.
          </p>
        </div>

      </div>


      <!-- ПІДПИСКА / МОБІЛЬНИЙ ДОДАТОК -->
      <div class="subscription-block">

        <h3 class="subtitle">Підписка N21 Mobile (Тест-драйв)</h3>

        <p class="text">
          Навчання починається не з лекцій, а з інтересу.  
          Концентрат міжнародного досвіду — у твоєму смартфоні.
        </p>

        <p class="text">
          Коротко, драйвово і без пафосу: це бібліотека реальних кейсів  
          і виступів міжнародних практиків успішного бізнесу.  
          Тренінги, мотивація та готові сценарії — доступні коли завгодно й де завгодно.
        </p>

        <h4 class="subtitle-sm">Унікальні переваги N21Mobile</h4>

        <ul class="list">
          <li>Велика бібліотека аудіо/відео від міжнародних підприємців.</li>
          <li>Ексклюзивний доступ для IBO у системі Network TwentyOne.</li>
          <li>Щомісячні програми підтримки й новий контент кожен місяць.</li>
          <li>Міжнародна інфраструктура: 40+ країн, 24 мови.</li>
          <li>350+ бізнес-зустрічей щотижня онлайн + офлайн.</li>
          <li>Доступність на iOS та Android.</li>
        </ul>

        <p class="text highlight">
          Спробуйте 30 днів безкоштовно, щоб відчути, як працює ваш персональний  
          бізнес- та лайф-навчальний простір від Network21.
        </p>

      </div>


      <!-- ВАРІАНТИ ДОСТУПУ -->
      <div class="pricing-block">
        <h3 class="subtitle">Після тесту — оберіть формат</h3>

        <div class="prices">

          <div class="price-card">
            <div class="price">₴300/міс</div>
            <div class="label">Базовий доступ</div>
          </div>

          <div class="price-card">
            <div class="price">₴500/міс</div>
            <div class="label">Розширений доступ</div>
          </div>

          <div class="price-card">
            <div class="price">₴750/міс</div>
            <div class="label">Професійний рівень</div>
          </div>

        </div>

        <p class="after-text">
          Якщо тест-драйв не підходить — залишайтесь учасником нашого Клубу.  
          Тут завжди є події, знайомства й ідеї, що заряджають.
        </p>
      </div>

    </div>
  </section>
</template>


<style scoped>
.join-wrapper {
  background-color: #15232C;
  padding: 20px 20px;
  display: flex;
  justify-content: center;
  width: 100%;
}

.join-container {
  width: 100%;
  max-width: 1150px;
}

/* Лінії */
.line-horizontal {
  width: 90%;
  height: 3px;
  margin: 20px auto;
  background-color: #3D4D55;
  border-radius: 2px;
}

/* Заголовок */
.block-title {
  text-align: center;
  color: white;
  font-size: 2.4rem;
  font-family: 'Playfair Display', serif;
}

/* Кроки */
.steps-block {
  background: #3D4D55;
  padding: 35px 30px;
  border-radius: 14px;
  margin-top: 40px;
  border-left: 4px solid #B58863;
}

.step {
  margin-bottom: 28px;
}

.step-number {
  font-size: 1.7rem;
  margin-bottom: 5px;
}

.step-title {
  color: white;
  margin-bottom: 6px;
  font-size: 1.4rem;
  font-family: 'Playfair Display', serif;
}

.step-text {
  color: #e6e6e6;
  font-size: 1.1rem;
  line-height: 1.6;
  font-family: 'Playfair Display', serif;
}

/* Підписка блок */
.subscription-block {
  background: #3D4D55;
  padding: 35px 30px;
  margin-top: 40px;
  border-radius: 14px;
  border-left: 4px solid #B58863;
}

.subtitle {
  font-size: 1.8rem;
  font-family: 'Playfair Display', serif;
  color: white;
  margin-bottom: 20px;
}

.subtitle-sm {
  font-size: 1.4rem;
  font-family: 'Playfair Display', serif;
  color: white;
  margin-top: 25px;
  margin-bottom: 12px;
}

.text {
  color: #e6e6e6;
  margin-bottom: 16px;
  font-size: 1.1rem;
  line-height: 1.6;
  font-family:'Playfair Display', serif;
}

/* Список */
.list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 22px 28px;
  padding: 0;
  margin: 40px 0;
  list-style: none;
}

.list li {
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
   border: 4px solid #283d4a;
}


/* Виділення */
.highlight {
  background: rgba(181, 136, 99, 0.1);
  border-left: 3px solid #B58863;
  padding: 10px 14px;
  border-radius: 8px;
}

/* Ціни */
.pricing-block {
  margin-top: 45px;
  text-align: center;
}

.prices {
  display: flex;
  gap: 18px;
  margin-top: 25px;
  justify-content: center;
  flex-wrap: wrap;
}

.price-card {
  background: #3D4D55;
  padding: 22px 30px;
  border-radius: 12px;
  border-top: 3px solid #B58863;
  width: 240px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.price-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.35);
}

.price {
  font-size: 1.8rem;
  color: #B58863;
  font-family: 'Playfair Display', serif;
}

.label {
  color: #e6e6e6;
  margin-top: 8px;
  font-size: 1.1rem;
}

.after-text {
  margin-top: 25px;
  color: #e6e6e6;
  font-size: 1.3rem;
  font-family: 'Playfair Display', serif;
}
</style>

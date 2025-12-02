<template>
  <div>
    <section class="start">
      <div class="header-bg">
        <NavigationBar />
      </div>

      <!-- Овальный блок с текстом -->
      <div class="intro-oval">
        У світі, де контакти формують реальність, ми створюємо платформу для 
        <span class="accent">тих, хто будує майбутнє своїми руками…</span>
      </div>
    </section>

    <!-- секции -->
    <section id="aboutUs" class="section about">
      <AboutUs />
    </section>

    <section id="Expirience" class="section experience">
      <UsMoments />
    </section>

    <section id="Price" class="section price">
      <AddToUs />
    </section>

    <section id="Contact" class="section contact">
      <ContactUs />
    </section>
    <section class="footer">
<FooterApp />
    </section>
  </div>
</template>

<script>
import NavigationBar from "@/components/NavigationBar.vue";
import AboutUs from "@/components/AboutUs.vue";
import UsMoments from "@/components/UsMoments.vue";
import AddToUs from "@/components/AddToUs.vue";
import ContactUs from "@/components/ContactUs.vue";
import FooterApp from "@/components/FooterApp.vue";

export default {
  name: "HomePage",
  components: { NavigationBar, AboutUs, UsMoments, AddToUs, ContactUs, FooterApp },
};
</script>

<style scoped>
/* === Header === */
.header-bg {
  background-color: #3D4D55;
  padding: 42px 0;
  display: flex;
  justify-content: center;
}

/* === Секции === */
.section {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 3rem;
  color: #161616;
}

.about { 
    background-color: #f0f0f0;
      min-height: auto;
 }
.experience { background-color: #d0d0d0; }
.price { background-color: #b0b0b0; }
.contact { background-color: #15232C; 
padding: 0;}

/* === Овальный блок с текстом === */
.intro-oval {
  position: absolute;
  bottom: 60px;
  left: 50%;
  transform: translateX(-50%);
  width: 80%;
  max-width: 900px;
  padding: 50px 60px; /* увеличены отступы сверху/снизу и слева/справа */

  background-color: #15232C;
  color: white;
  font-size: 1.6rem;
  text-align: center;
  border-radius: 40px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.25);
  font-family: 'Playfair Display', serif;
  line-height: 1.5;
  backdrop-filter: blur(2px);
}

/* === Start background === */
.start {
  position: relative;
  background-image: url("@/assets/logoGreat.PNG");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  width: 100%;
  height: 100vh;
}

/* === Акцентный текст === */
.accent {
  text-decoration: underline;
  text-decoration-color: #B58863;
  text-underline-offset: 6px;
  font-weight: 600;
}

/* === Мобильная версия (до 480px) === */
@media (max-width: 480px) {
  .section {
    font-size: 2rem;
  }

  .intro-oval {
    width: 80%;
    padding: 30px 20px; /* увеличены внутренние отступы для воздуха вокруг текста */
    font-size: 1.4rem;
    line-height: 2.2;
    bottom: 50px; /* чуть выше от нижнего края */
  }

  .accent {
    text-underline-offset: 4px;
  }

  .header-bg {
    padding: 30px 0;
  }
}
</style>

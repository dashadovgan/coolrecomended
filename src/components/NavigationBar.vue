<template>
  <nav class="navbar">
    <!-- Логотип -->
   
  

    <!-- Затемнение фона при открытии меню -->
    <div v-if="isMenuOpen" class="menu-overlay" @click="closeMenu"></div>

    <!-- Бургер -->
    <div class="burger" :class="{ active: isMenuOpen }" @click="toggleMenu">
      <div></div>
      <div></div>
      <div></div>
    </div>

    <!-- Меню -->
    <ul :class="['nav-links', { active: isMenuOpen }]">
      <li><a @click="scrollTo('aboutUs')">Про нас</a></li>
      <li><a @click="scrollTo('Expirience')">Наш досвід</a></li>
      <li><a @click="scrollTo('Price')">Як до нас доеднатися</a></li>
      <li><a @click="scrollTo('Contact')">Контакти</a></li>
      
</ul>
      <!-- Кнопка внутри меню (только на телефоне) -->
      

    <!-- Кнопка на десктопе -->
   
  </nav>
</template>

<script>


export default {
  name: "AppNavbar",

  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    closeMenu() {
      this.isMenuOpen = false;
    },
    scrollTo(id) {
      const section = document.getElementById(id);
      if (section) {
        section.scrollIntoView({ behavior: "smooth" });
      }
      this.isMenuOpen = false;
    },
  },
};
</script>

<style scoped>
.timeButton {
  display: none;
}

ul {
  padding: 0;
  margin: 0;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 12px;
  background-color: transparent;
  position:absolute;
  top: 0;
  left: 15%;
  width: 100%;
  z-index: 1000;
}



/* Десктопное меню */
.nav-links {
  display: flex;
  gap: 200px;
  list-style: none;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: #15232C;
  border-radius: 30px;
  padding: 15px 25px;
    border: 2px solid #B58863;
}

.nav-links li a {
  text-decoration: none;
  color: white;
  font-weight: 400;
  cursor: pointer;
  font-family: 'Playfair Display', serif;
  font-weight: 400;
}

.nav-links li a:hover {
  color: white;
  font-weight: 600;
  font-size: 16px;
}

.action-button {
  display: flex;
  margin-right: 50px;
  font-weight: 400;
  font-size: 16px;
}

.action-button:hover {
  font-weight: 600;
}

.burger {
  display: none;
}

/* --- MOBILE VERSION --- */
@media (max-width: 500px) {
  .nav-links {
    position: fixed;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    flex-direction: column;
    background-color: #010614;
    gap: 32px;
    display: none;
    z-index: 1000;
    border-radius: 0;
    padding-top: 120px; /* отступ сверху, чтобы ссылки были "вверху" */
    justify-content: flex-start; /* ссылки начинаются сверху */
    align-items: center;          /* по горизонтали центр */
  }

  .nav-links.active {
    display: flex;
  }

  .nav-links li a {
    font-size: 30px;
    color: white;
  }

  .burger {
    display: flex;
    flex-direction: column;
    gap: 5px;
    cursor: pointer;
    z-index: 1001;
    position: fixed;
    top: 15px;
    left: 15px;
  }

  .burger div {
    width: 30px;
    height: 4px;
    background-color: #fff;
    border-radius: 2px;
    transition: all 0.3s ease;
    transform-origin: center;
  }

  .burger.active div:nth-child(1) {
    transform: rotate(45deg) translate(7px, 7px);
  }
  .burger.active div:nth-child(2) {
    opacity: 0;
  }
  .burger.active div:nth-child(3) {
    transform: rotate(-45deg) translate(5px, -5px);
  }

  .menu-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-color: rgba(1,6,20,0.95);
    z-index: 999;
  }
}


</style>
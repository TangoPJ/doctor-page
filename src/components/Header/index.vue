<template>
  <header class='header'>
    <div class="bg" :style="{ backgroundImage: `url(${headerBackgroundImage})` }"></div>
    <div class="header__content">
      <h1 class="header__title">Персональный врач</h1>
      <h2 class="header__subtitle">Добро пожаловать на официальный сайт персонального врача. Квалифицированный специалист помогает поддерживать ваше здоровье</h2>
      <button class="header__button">Записаться на прием</button>
    </div>
  </header>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Header',

  setup() {
    const headerBackgroundImage = `${process.env.VUE_APP_MEDIA_FROM_S3}/header-bg.jpeg`

    return {
      headerBackgroundImage,
    }
  },
})
</script>

<style lang="scss" scoped>
.header {
  height: 100vh;
  position: relative;
  z-index: 2;
  color: #424242;

  &__content {
    width: 1100px;
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 8;
  }

  &__title {
    font-size: 68px;
    font-weight: 500;
    margin-bottom: 10px;
    width: 100%;
  }

  &__subtitle {
    font-size: 24px;
    margin-bottom: 38px;
    font-weight: normal;
    color: #000000;
  }

  &__button {
    background-color: #71b6f9;
    border-radius: 2em;
    box-shadow: 0;
    font-size: 18px;
    border: none;
    width: 350px;
    height: 60px;
    line-height: 60px;
    color: #ffffff;
    overflow: hidden;
    transition: .3s;
    cursor: pointer;
  }
}

.bg {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  opacity: 0.5;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  z-index: 3;
}
</style>

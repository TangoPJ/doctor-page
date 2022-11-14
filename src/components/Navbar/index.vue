<template>
  <div class="wrapper">
    <div class="navbar">
      <a href="/">
        <img :src="logo" width="100" height="50" alt="Aybek Usambaev" class="navbar__logo">
      </a>
      <div class="right-side">
        <ul class="menu">
          <li class="menu__item" v-for="{ id, name, url } in items" :key="`${id}-${name}`">
            <a class="menu__link" :href="url">{{ name }}</a>
          </li>
        </ul>
        <a class="phone" href="tel:996555240064">+966 555 240064</a>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import { items } from '@/data/items'

export default defineComponent({
  name: 'Navbar',

  setup() {
    const logo = `${process.env.VUE_APP_MEDIA_FROM_S3}/logo.svg`
    console.log(logo)

    return {
      logo,
      items,
    }
  }
})
</script>

<style lang="scss" scoped>
.wrapper {
  background: #edf5fd;
  padding: 7px 25px;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  z-index: 9;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1170px;
  margin: 0 auto;

  &__logo {
    max-width: 200px;
    display: block;
    width: 100%;
    height: auto;
  }

  @media screen and (max-width: 1100px) {
    flex-direction: column;
    flex-wrap: wrap;
  }
}

.right-side {
  display: flex;
  align-items: center;

  @media screen and (max-width: 860px) {
    flex-direction: column;
  }
}

.menu {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;

  &__item {
    margin: 5px 0;
  }

  &__item:last-child {
    padding-right: 10px;
    border-right: 1px solid orange;

    @media screen and (max-width: 867px) {
      padding-right: 0;
      border: none;
    }
  }

  &__item:not(:first-child) {
    margin-left: 10px;

    &::before {
      content: "○";
      font-size: 12px;
      padding-right: 10px;
      position: relative;
      top: -3px;
    }
  }

  &__link {
    &:hover {
      text-decoration: underline;
    }
  }

  @media screen and (max-width: 365px) {
    font-size: 14px;

    &__item {
      margin: 3px 0;
    }
  }
}

.phone {
  margin-left: 10px;

  &:hover {
    color: orange;
  }

  @media screen and (max-width: 865px) {
    margin-left: 0;
  }
}
</style>

<template>
  <div class="cart cart--empty">
    <h2>Корзина пустая <icon>😕</icon></h2>
    <p>
      Вероятней всего, вы не заказывали ещё пиццу.<br />
      Для того, чтобы заказать пиццу, перейди на главную страницу.
    </p>
    <img :src="emptyCart" alt="Empty cart" />
    <router-link :to="{ name: 'Home' }" class="button button--black">
      <span>Вернуться назад</span>
    </router-link>
  </div>
</template>

<script>
import emptyCart from '@/assets/img/empty-cart.png'

export default {
  setup() {
    return { emptyCart }
  },
}
</script>

<style></style>

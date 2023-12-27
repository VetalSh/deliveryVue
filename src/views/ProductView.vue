<template>
  <section class="products">
    <div class="container">
      <div class="products-wrapper" id="products-container">
        <div class="products-card" v-for="good in goodsArray" :key="good.id">
          <div class="products-card__image">
            <img :src="getUrl(good.image)" alt="goods-1" />
          </div>
          <div class="products-card__description">
            <div class="products-card__description-row">
              <h5 class="products-card__description--name">
                {{ good.title }}
              </h5>
            </div>
            <div class="products-card__description-row">
              <p class="products-card__description--text">
                {{ good.description }}
              </p>
            </div>
            <div class="products-card__description-row">
              <div class="products-card__description-controls">
                <button class="btn btn-primary">
                  <span>В корзину</span>
                  <img src="../assets/img/icons/cart-white.svg" alt="cart" />
                </button>
                <span class="products-card__description-controls--price"
                  >{{ good.price }} грн.</span
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { goodsArray } from "../constants/products";

const getUrl = (name) => {
  return new URL(`../assets/img/${name}`, import.meta.url);
};
</script>

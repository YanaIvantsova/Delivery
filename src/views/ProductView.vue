<template>
  <section class="products">
    <div class="container">
      <div class="products-wrapper" id="products-container">
        <div
          class="products-card"
          v-for="product in productsArray"
          :key="product.id"
        >
          <div class="products-card__image">
            <img :src="getUrl(product.image)" alt="goods1-image" />
          </div>
          <div class="products-card__description">
            <div class="products-card__description-row">
              <h5 class="products-card__description--name">
                {{ product.name }}
              </h5>
            </div>
            <div class="products-card__description-row">
              <p class="products-card__description--text">
                {{ product.description }}
              </p>
            </div>
            <div class="products-card__description-row">
              <div class="products-card__description--controls">
                <button class="btn btn-primary">
                  В корзину<img
                    src="../assets/images/items/shopping-cart-white.svg"
                    alt="cart-icon"
                  />
                </button>
                <span class="products-card__description-controls--price"
                  >{{ product.price }} ₽</span
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
import { productsArray } from "../constants/products";

const getUrl = (name) => {
  console.log("hello");
  console.log(name);
  return new URL(`../assets/images/goods/${name}`, import.meta.url);
};
</script>
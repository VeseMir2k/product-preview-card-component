<template>
  <section class="card">
    <div class="card__header">
      <picture>
        <source media="(min-width:632px)" srcset="./images/image-product-desktop.jpg" />
        <img class="card__image" src="./images/image-product-mobile.jpg" alt="image product"
      /></picture>
    </div>
    <div class="card__main">
      <span class="card__category">PERFUME</span>
      <h1 class="card__title">Gabrielle Essence Eau De Parfum</h1>
      <p class="card__description">
        A floral, solar and voluptuous interpretation composed by Olivier Polge, Perfumer-Creator
        for the House of CHANEL.
      </p>
      <div class="card__price">$149.99 <span class="card__old-price">$169.99</span></div>
      <button class="card__button">
        <img class="card__icon" src="./images/icon-cart.svg" alt="" />Add to Cart
      </button>
    </div>
  </section>
</template>

<style scoped>
.card {
  background-color: var(--white-color);
  border-radius: 10px;
  color: var(--aurometal-saurus-color);
  font-family: var(--montserrat-font);
  overflow: hidden;
  width: 100%;
  display: flex;
  flex-direction: column;
}

.card__image {
  width: 100%;
}

.card__main {
  padding: 24px;
}

.card__category {
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 5px;
}

.card__title {
  color: var(--gunmetal-color);
  font-family: var(--fraunces-font);
  font-size: 32px;
  font-weight: 700;
  line-height: 32px;
  margin: 12px 0 16px;
}

.card__description {
  font-size: 14px;
  line-height: 23px;
}

.card__price {
  color: var(--deep-aquamarine-color);
  font-family: var(--fraunces-font);
  font-size: 32px;
  font-weight: 700;
  line-height: 32px;
  margin: 24px 0 20px;
  position: relative;
}

.card__old-price {
  color: var(--aurometal-saurus-color);
  font-size: 13px;
  font-weight: 500;
  line-height: 23px;
  margin-left: 20px;
  position: absolute;
  text-decoration: line-through;
  top: 5px;
}

.card__button {
  background-color: var(--deep-aquamarine-color);
  border: 0;
  border-radius: 8px;
  color: var(--white-color);
  cursor: default;
  display: flex;
  font-size: 14px;
  font-weight: bold;
  gap: 12px;
  justify-content: center;
  padding: 15px 0;
  width: 100%;
}

.card__button:hover {
  background-color: var(--deep-aquamarine-hover-color);
}

@media (min-width: 632px) {
  .card {
    width: 600px;
    flex-direction: row;
  }
  .card__header {
    width: 50%;
  }

  .card__image {
    height: 100%;
  }

  .card__main {
    width: 50%;
    padding: 32px;
  }

  .card__title {
    margin: 20px 0 24px;
  }

  .card__price {
    margin: 30px 0;
  }
}
</style>

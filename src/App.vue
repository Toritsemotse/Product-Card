<template>
  <main>
    <div class="container">
      <div class="img"></div>
      <div class="text">
        <p class="perfume">PERFUME</p>
        <div class="title">
          <h2>Gabrielle Essence Eau De Parfum</h2>
        </div>
        <p>A floral, solar and voluptuous interpretation composed by Oliver Polge, Perfumer-Creator for the House of
          CHANEL </p>
        <div class="prices">
          <div class="first-price">
            <h1>$149.99</h1>
          </div>
          <div class="second-price">
            <p>$169.99</p>
          </div>
        </div>
        <div class="cart">
          <div class="cart-img"></div>
          <div class="cart-text">
            <p>Add to cart</p>
          </div>
        </div>
      </div>

    </div>
  </main>
</template>

<style scoped>
main {
  background-image: url("");
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: hsl(30, 38%, 92%);
}

.container {
  background-color: hsl(0, 0%, 100%);
  width: 600px;
  height: 450px;
  border-radius: 10px;
  display: flex;
}

.img {
  height: 100%;
  width: 50%;
  background-repeat: no-repeat;
  background-image: url("/images/image-product-desktop.jpg");
  background-size: cover;
  border-bottom-left-radius: 10px;
  border-top-left-radius: 10px;
}

.text {
  width: 50%;
  height: 100%;
  padding: 30px;
}

.perfume {
  font-family: "Montserrat";
  font-weight: 500;
  letter-spacing: 5px;
  font-size: 12px
}

.title {
  padding-right: 20px;
}

h2 {
  font-size: 30px;
  font-weight: 700;
  line-height: 30px;
  font-family: "Fraunces", sans-serif;
  margin-top: 20px;
  margin-bottom: 20px;

}

p {
  font-weight: 500;
  font-family: "Montserrat";
  color: hsl(228, 12%, 48%);
}

.prices {
  display: flex;
  align-items: center;
  margin-top: 20px;
}

.first-price {
  margin-right: 20px;
  color: hsl(158, 36%, 37%);
}

h1 {
  font-weight: 700;
  font-family: "Fraunces";
}

.second-price {
  text-decoration: line-through;
}

.cart {
  width: 100%;
  height: 55px;
  background-color: hsl(158, 36%, 37%);
  border-radius: 10px;
  margin-top: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
}

.cart:hover {
  cursor: pointer;
}

.cart-img {
  background-image: url("/images/icon-cart.svg");
  background-size: contain;
  background-repeat: no-repeat;
  width: 18px;
  height: 18px;
  margin-right: 10px;
}

.cart-text p {
  color: white;
}

@media (max-width:600px) {

  main {
    padding-inline: 20px;
  }

  .container {
    flex-direction: column;
    width: 100%;
    height: auto;
    border-radius: 10px;
    overflow: hidden;
  }

  .img {
    height: 280px;
    width: 100%;
    background-repeat: no-repeat;
    background-image: url("/images/image-product-mobile.jpg");
    background-size: cover;
    border-radius: 0px;
  }

  .text{
    width: 100%;
    height: fit-content;
  }

}
</style>
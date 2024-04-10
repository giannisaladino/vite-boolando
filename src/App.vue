<script>
import AppHeader from "./components/AppHeader.vue"
import AppFooter from "./components/AppFooter.vue"
export default {
  components: {
    AppHeader,
    AppFooter,
  },
}
</script>

<template>
  <div>
    <AppHeader />
  </div>

  <main class="page-content">
    <div class="section">
      <div class="container">
        <div class="row">
          <div class="col-4">
            <div class="card">
              <div class="card-header">
                <img src="/img/1.webp" alt="">
                <span class="price-badge">-50 %</span>
                <span class="tag-badge">Sostenibilità</span>
                <span class="heart-badge">&hearts;</span>
                <div class="overlay">
                  <img src="/img/1b.webp" alt="">
                </div>
              </div>
              <div class="card-body">
                <p>Levi's</p>
                <p><strong>RELAXED FIT TEE UNISEX</strong></p>
                <p class="red-price"><strong>14,99&euro;</strong></p><span class="before-price">29,99&euro;</span>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card product">
              <div class="card-header">
                <img src="/img/2.webp" alt="">
                <span class="price-badge">-30 %</span>
                <span class="heart-badge">&hearts;</span>
                <div class="overlay">
                  <img src="/img/2b.webp" alt="">
                </div>
              </div>
              <div class="card-body">
                <p>Guess</p>
                <p><strong>ROSES TEE</strong></p>
                <p class="red-price"><strong>20,99&euro;</strong></p><span class="before-price">29,99&euro;</span>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card product">
              <div class="card-header">
                <img src="/img/3.webp" alt="">
                <span class="price-badge">-30 %</span>
                <span class="heart-badge">&hearts;</span>
              </div>
              <div class="card-body">
                <p>Come Zucchero Filato</p>
                <p><strong>VOGLIA DI COLORI PASTELLO</strong></p>
                <p class="red-price"><strong>129,99&euro;</strong></p><span class="before-price">184,99&euro;</span>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card product">
              <div class="card-header">
                <img src="/img/4.webp" alt="">
                <span class="price-badge">-50 %</span>
                <span class="tag-badge">Sostenibilità</span>
                <span class="heart-badge">&hearts;</span>
                <div class="overlay"><img src="/img/4b.webp" alt=""></div>
              </div>
              <div class="card-body">
                <p>Levi's</p>
                <p><strong>TEE UNISEX</strong></p>
                <p class="red-price"><strong>14,99&euro;</strong></p><span class="before-price">29,99&euro;</span>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card product">
              <div class="card-header">
                <img src="/img/5.webp" alt="">
                <span class="heart-badge">&hearts;</span>
                <div class="overlay"><img src="/img/5b.webp" alt=""></div>
              </div>
              <div class="card-body">
                <p>Maya Deluxe</p>
                <p><strong>STRIPE BODICE</strong></p>
                <p class="red-price"><strong>99,99&euro;</strong></p>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card product">
              <div class="card-header">
                <img src="/img/6.webp" alt="">
                <span class="tag-badge only">Sostenibilità</span>
                <span class="heart-badge">&hearts;</span>
                <div class="overlay"><img src="/img/6b.webp" alt=""></div>
              </div>
              <div class="card-body">
                <p>Esprit</p>
                <p><strong>MAGLIONE - BLACK</strong></p>
                <p class="red-price"><strong>29,99&euro;</strong></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>

  <div>
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use "./style/general";

/* STYLE */

.page-header {
  background-color: #FF6801;
  color: white;
}

.page-header .row {
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}

.logo-header {
  height: 25px;
}

.red-price {
  display: inline-block;
  color: red;
  padding-right: 4px;
}

.before-price {
  text-decoration: line-through;
}

.card-header {
  position: relative;
}

.card-header>img {
  display: block;
}

.card-body p,
span {
  font-size: 14px;
}

.card-header .price-badge {
  position: absolute;
  bottom: 30px;
}

.card-header .tag-badge {
  position: absolute;
  bottom: 30px;
  left: 45px;
}

.card-header .only {
  position: absolute;
  bottom: 30px;
  left: 0px;
}

.card-header .heart-badge {
  position: absolute;
  top: 20px;
  right: 0;
}

.price-badge {
  background-color: #FF0000;
  color: white;
  padding: 0 5px;
  font-size: 13px;
}

.tag-badge {
  background-color: #008001;
  color: white;
  padding: 0 6px;
  font-size: 13px;
}

.heart-badge {
  background-color: white;
  font-size: 20px;
  padding: 9px;
}

.card-header .overlay {
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
  transition: 500ms;
}

.card-header:hover .overlay {
  opacity: 1;
  z-index: 20;
}
</style>

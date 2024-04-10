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
</style>

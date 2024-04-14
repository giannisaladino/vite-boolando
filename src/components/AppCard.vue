<script>
export default {
    props: ['product'],
    data() {
    }
}
</script>

<template>
    <div class="card product">
        <div class="card-header">
            <img :src="'/img/' + product.frontImage" alt="">
            <span class="price-badge">-50 %</span>
            <span class="tag-badge">Sostenibilità</span>
            <span class="heart-badge">&hearts;</span>
            <div class="overlay">
                <img :src="`/img/${product.backImage}`" alt="">
            </div>
        </div>
        <div class="card-body">
            <p>{{ product.brand }}</p>
            <p><strong>{{ product.name }}</strong></p>
            <p class="red-price"><strong>14,99&euro;</strong></p>
            <span class="before-price"> {{ product.price }} &euro;</span>
        </div>
    </div>
</template>

<style>
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
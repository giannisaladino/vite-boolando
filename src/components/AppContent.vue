<script>
import AppCard from "./AppCard.vue";
import data from "../assets/db.json"
export default {
    components: {
        AppCard
    },
    data() {
        return {
            products: data.products
        }
    }
}
</script>

<template>
    <main class="page-content">
        <div class="section">
            <div class="container">
                <div class="row">
                    <div v-for="product in products" :key="product.id" class="col-4">
                        <AppCard :product="product" />
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
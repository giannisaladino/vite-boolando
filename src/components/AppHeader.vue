<script>
export default {
    data() {
    }
}
</script>

<template>
    <header class="page-header">
        <nav class="container">
            <div class="row">
                <ul class="flex">
                    <li>Donna</li>
                    <li>Uomo</li>
                    <li>Bambini</li>
                </ul>
                <img class="logo-header" src="/img/boolean-logo.png" alt="">
                <ul class="flex">
                    <li>&hearts;</li>
                    <li>&hearts;</li>
                    <li>&hearts;</li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style>
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

</style>
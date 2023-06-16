<script setup>

</script>

<template>
    <div class="card card-shadow special">
        <div class="header">
            <p class="title">Best Selling</p>
            <div class="percent">
                <span>94%</span>
            </div>
        </div>
        <div class="best-day">
            <span class="day">Tuesday</span>
            <span class="amoung">215,523 pcs</span>
        </div>
        <div class="chart">
            <div class="pie-chart">
                <img src="" alt="">
            </div>
        </div>

    </div>
</template>
<style scoped>
.card.special {
    color: white;
    background: linear-gradient(113.24deg, #13B497 16.01%, #05737A 106.71%);
    display: none;
}

@media (min-width: 578px) {
    .card.special {
        display: flex;
    }
}

@media (min-width: 768px) {}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>
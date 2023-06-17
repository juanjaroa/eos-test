<script setup>

</script>

<template>
    <div class="card card-shadow special">
        <div class="header">
            <div>
                <p class="title">Sales Comparison</p>
                <div class="wrap"><span class="sub">Than last day</span></div>

            </div>
            <div class="percent">
                <span>94%</span>
            </div>
        </div>

        <div class="chart">
            <div class="pie-chart">
                <img src="../content/assets/barChar-especial.png" alt="">
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

.card .header {
    align-items: center;
    padding: 1rem 3rem 0 2rem;
}

.header .title {
    font-size: 1.25rem;
    font-weight: 600;
    opacity: 0.91;
}

.header .wrap {
    position: relative;
    height: 0;
    opacity: 0.91;
}

header .sub {
    position: absolute;
}

.percent span {
    font-size: 2.5rem;
    font-weight: 600;
}

@media (min-width: 578px) {}

@media (min-width: 768px) {
    .card.special {
        display: flex;
    }
}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>
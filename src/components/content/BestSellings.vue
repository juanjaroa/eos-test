<script setup>

</script>

<template>
    <div class="card card-shadow">
        <div class="header">
            <p class="title">Best Selling</p>
            <div class="filter">
                <span class="label">This week</span>
                <img src="../../assets/ic_chevron.png" alt="">
            </div>
        </div>
        <div class="best-day">
            <span class="day">Tuesday</span>
            <span class="amoung">215,523 pcs</span>
        </div>

        <div class="charts">
            <div class="pie-chart">
                <img src="./assets/pieChart.png" alt="">
            </div>
            <div class="bar-char">
                <img src="./assets/barChart3.png" alt="">
            </div>
        </div>

    </div>
</template>

<style scoped>
.header .title {
    font-size: 1rem;
    font-weight: 300;
    line-height: 1.6em;
}

.day-cipher {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
}


.best-day {
    background: #20262D;
    padding: 7.5px 12px;
    display: flex;
    justify-content: space-between;
    align-content: center;
    border-radius: 7px;
}

.best-day .day,
.best-day .amoung {
    font-size: 8px;
}

.charts {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
    width: 100%;
    padding-top: 2rem;
}

.charts>div {
    display: flex;
    justify-content: center;
    align-content: center;
    flex-direction: column;
}

.charts>div:last-child {
    display: none;
}

.charts img {
    width: 100%;
    height: auto;
    display: block;
}

@media (min-width: 578px) {}

@media (min-width: 768px) {


    .header .title {
        font-size: 1.5rem;
        font-weight: 500;
        line-height: 1.6em;
    }

    .best-day .day,
    .best-day .amoung {
        font-size: 1rem;
    }



    .charts {
        flex-direction: row;

    }

    .charts>div:first-child {
        width: 58%;
    }

    .charts>div:last-child {
        display: flex;
        width: 42%;
        justify-content: start;
        padding-top: 0.5rem;
    }
}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>
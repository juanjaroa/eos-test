<script setup>

</script>

<template>
    <div id="cards-grid">
        <!-- Card one -->
        <div class="card card-shadow">
            <div class="header">
                <div class="card-title">
                    <p class="title">456k Pcs</p>
                    <p class="subtitle">Ticket Sold</p>
                </div>
                <div class="filter">
                    <span class="label">Daily</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
            <div class="progress">
                <div class="progress-value"></div>
            </div>
        </div>
        <!-- Card two -->
        <div class="card card-shadow aspect-ratio">
            <div class="header">
                <div class="card-title">
                    <p class="title">451,509</p>
                    <p class="subtitle">Sales</p>
                </div>
                <div class="filter">
                    <span class="label">This Week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
            <img class="card-mask" src="../assets/curveChart.png" alt="">
        </div>
        <!-- Card three -->
        <div class="card card-shadow aspect-ratio">
            <div class="header">
                <div class="card-title">
                    <p class="title">$456,623</p>
                    <p class="subtitle">Income</p>
                </div>
                <div class="filter">
                    <span class="label">Monthly</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
            <img class="card-mask" src="../assets/doublecurveChart.png" alt="">
        </div>
        <!-- Card four -->
        <div class="card card-shadow no-title">
            <div class="header">
                <div class="card-title">
                </div>
                <div class="filter">
                    <span class="label">This Week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
            <div class="chart-alt">
                <img class="chart" src="../assets/pieChart-alt.png" alt="">
                <img class="legend" src="../assets/legend.png" alt="">
            </div>
        </div>

    </div>
</template>
<style scoped>
#cards-grid {
    display: grid;
    grid-gap: 1.5rem;
}

.card {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    padding: 1.25rem 1.5rem;
    position: relative;
    overflow: hidden;
}

.card.aspect-ratio {
    aspect-ratio: 7 / 2.5;
}

.card-title {
    display: flex;
    flex-direction: column;
}

.card-title .title {
    font-size: 1rem;
    font-weight: 600;
    line-height: 1.5em;
}

.card-title .subtitle {
    font-size: 0.75rem;
    font-weight: 300;
    line-height: 1.5em;
    opacity: 0.6;
}

.progress {
    display: block;
    height: 0.8rem;
    position: relative;
    /* overflow: hidden; */
    margin-top: auto;
}

.progress-value {
    display: block;
    background: rgba(255, 255, 255, 0.12);
    border-radius: 40px;
    height: 0.8rem;
    z-index: 1;
    position: relative;
    width: 100%;
}

.progress::before {
    position: absolute;
    display: block;
    content: '';
    border-radius: 40px;
    height: 100%;
    width: 80%;
    z-index: 0;
    top: 0;
    box-shadow: 0px 0px 16.7552px rgba(19, 180, 151, 0.56)
}

.progress::after {
    position: absolute;
    display: block;
    content: '';
    border-radius: 40px;
    background: #13B497;
    height: 100%;
    width: 80%;
    top: 0;
    z-index: 9;
}

.card-mask {
    position: absolute;
    width: 100%;
    left: 0;
    right: 0;
    bottom: 0;
}

.chart-alt {
    display: flex;
    align-items: baseline;
    gap: 1.5rem;
    margin-top: auto;
}

.chart-alt .chart {
    width: 40%;
    margin: 0 auto
}

.chart-alt .legend {
    width: 60%;
}

.no-title .header {
    margin: 0 !important;
    position: relative;
}

.no-title {
    gap: 0 !important
}

.no-title .filter {
    display: none;
    position: absolute;
    right: 0;
}

.no-title .chart-alt .legend {
    display: none;
}


@media (min-width: 578px) {
    .card.aspect-ratio {
        aspect-ratio: 7 / 2;
    }

    .no-title .filter {
        display: flex;
    }

    .no-title .chart-alt .legend {
        display: block;
    }
}

@media (min-width: 768px) {
    #cards-grid {
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr;
    }

    .card .header {
        margin-bottom: 0.5rem;
    }

    .card {
        /* padding: 2rem 1.75rem; */

    }

    .card.aspect-ratio {
        aspect-ratio: initial;
    }


}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>
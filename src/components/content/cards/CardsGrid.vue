<script setup>

</script>

<template>
    <div id="cards-grid">
        <div class="card card-shadow">
            <div class="header">
                <p class="title">Best Selling</p>
                <div class="filter">
                    <span class="label">This week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
        </div>
        <div class="card card-shadow">
            <div class="header">
                <p class="title">Best Selling</p>
                <div class="filter">
                    <span class="label">This week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
        </div>
        <div class="card card-shadow">
            <div class="header">
                <p class="title">Best Selling</p>
                <div class="filter">
                    <span class="label">This week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
        </div>
        <div class="card card-shadow">
            <div class="header">
                <p class="title">Best Selling</p>
                <div class="filter">
                    <span class="label">This week</span>
                    <img src="../../../assets/ic_chevron.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
#cards-grid {
    display: grid;
    grid-gap: 2rem;

}


@media (min-width: 578px) {}

@media (min-width: 768px) {
    #cards-grid {
        grid-template-columns: 1fr 1fr;
    }
}

@media (min-width: 992px) {}

@media (min-width: 1200px) {}

@media (min-width: 1400px) {}
</style>
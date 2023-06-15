<script setup>
import NavBar from './components/navbar/NavBar.vue';
import BestSellings from './components/content/BestSellings.vue';
import MiscellaneousCards from './components/content/cards/MiscellaneousCards.vue';
import SalesComparison from './components/content/SalesComparison.vue';
import EventGalleries from './components/content/EventGalleries.vue'

</script>

<template>
  <div id="wrap-root">
    <NavBar />
    <div class="breadcrumbs">Dashboard /</div>
    <div class="container">
      <div class="column">
        <section id="best-selling">
          <BestSellings />
        </section>
        <section id="miscellaneous">
          <MiscellaneousCards />
        </section>
      </div>
      <div class="column">
        <section id="Sales-comparison">
          <SalesComparison />
        </section>
        <section id="event-galleries">
          <EventGalleries />
        </section>
      </div>
    </div>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap');

body {
  background: #24292E;
  color: #FFFFFF;
  font-family: 'Poppins', sans-serif;
  min-height: 100vh;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
}

#wrap-root {
  height: 100%;
}

.breadcrumbs {
  width: 100%;
  padding: 19px 90px;
  background: #2D3339;
  color: #13B497;
  font-weight: 600;
}

.container {
  width: 100%;
  margin: 0px auto;
  padding: 1rem;
}

@media (min-width: 578px) {
  .container {
    max-width: 578px;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 768px;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 992px;
  }
}

@media (min-width: 1200px) {
  .container {
    max-width: 1200px;
  }
}

@media (min-width: 1400px) {
  .container {
    max-width: 1400px;
  }
}
</style>

<script setup>
import NavBar from './components/navbar/NavBar.vue';
import BestSellings from './components/content/BestSellings.vue';
import CardsGrid from './components/content/cards/CardsGrid.vue';
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
          <CardsGrid />
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
  display: none;
  width: 100%;
  padding: 19px 90px;
  background: #2D3339;
  color: #13B497;
  font-weight: 600;
}

.container {
  width: 100%;
  margin: 0px auto;
  padding: 1rem 1rem 2rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.card {
  background: #272E35;
  border-radius: 15px;
  display: flex;
  flex-direction: column;
  padding: 15px 15px 20px;
}

.card .header {
  display: flex;
  width: 100%;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 0.5rem;
}

.card .filter {
  display: flex;
  width: max-content;
  gap: 1px;
  align-items: center;
  cursor: pointer;
}

.card .filter .label {
  font-size: 0.5rem;
  color: #B7B7B7;
}

.card .filter img {
  width: 12px;
}


.card-shadow {
  box-shadow: 0px 6px 11px rgba(62, 73, 84, 0.04);
}

.column {
  display: flex;
  flex-direction: column;
  gap: 1.6rem;
}

#event-galleries {
  flex-grow: 1;
  aspect-ratio: 1 / 1;
}

button,
img.chevron {
  cursor: pointer;
}

@media (min-width: 578px) {
  .container {
    max-width: 578px;
    padding: 1rem 1rem 3rem;
  }

  .card .filter .label {
    font-size: 0.75rem;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 768px;
    padding: 3rem 1rem;
  }

  .breadcrumbs {
    display: flex;
  }

  .card .header {
    margin-bottom: 1rem;
  }

  .card .filter img {
    width: 1.75rem;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 992px;
    flex-direction: row;
  }

  .column {
    width: 50%;
  }

  #event-galleries {
    aspect-ratio: initial;
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

@media (min-width: 1600px) {
  .container {
    max-width: 1600px;
  }
}

@media (min-width: 1920px) {
  .container {
    max-width: 1920px;
  }
}
</style>

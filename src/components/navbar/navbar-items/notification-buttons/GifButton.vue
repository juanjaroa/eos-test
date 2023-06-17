<script setup></script>
<template>
    <button>
        <img class="icon" src="../../assets/ic_gif.png" alt="">
        <div class="badge"></div>
    </button>
</template>

<style scoped>
button {
    display: none;
}

.badge {
    background: #647280;
}

@media (min-width: 768px) {
    button {
        display: flex;
    }
}
</style>
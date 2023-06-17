<script setup></script>
<template>
    <button>
        <img class="icon" src="../../assets/ic_chat.png" alt="">
        <div class="badge"></div>
    </button>
</template>

<style scoped>
button {
    display: none;
}

@media (min-width: 768px) {
    button {
        display: flex;
    }
}
</style>
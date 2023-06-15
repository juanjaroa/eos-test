<script setup>
import AlertButton from './notification-buttons/AlertButton.vue';
import ChatButton from './notification-buttons/ChatButton.vue';
import GifButton from './notification-buttons/GifButton.vue';
</script>
<template>
    <div id="notification-buttons">
        <AlertButton />
        <ChatButton />
        <GifButton />
    </div>
</template>

<style scoped>
#notification-buttons {
    display: flex;
    gap: 22px;
}
</style>
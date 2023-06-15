<script setup>

</script>

<template>
    <div id="field">
        <input type="text" placeholder="  Search here">
        <img src="../assets/search.png" alt="">
    </div>
</template>

<style scoped>
#field {
    position: relative;
    display: flex;
    align-items: center;
    height: 36px;
}

#field img {
    position: absolute;
    right: 16px;
    width: 16px;
    height: auto;
}

input {
    background: #1C2126;
    border: 1px solid #2F363D;
    border-radius: 12px;
    font-size: 12px;
    padding: 8px 48px 8px 16px;
    caret-color: #13B497;
    height: 100%;
    width: 25vw;
}

input::placeholder {
    color: #B9B9B9;
}

@media (min-width: 768px) {
    #field {
        height: 100%;
    }

    input {
        font-size: 16px;
        padding: 16px 74px 16px 24px;
        width: 25vw;
    }

    #field img {
        right: 25px;
        width: 24px;
    }
}
</style>
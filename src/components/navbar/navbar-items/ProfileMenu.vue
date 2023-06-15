<script setup>

</script>
<template>
    <div id="profile">
        <img id="profile-pic" src="../assets/profile_pic.png" alt="">
        <span class="profile-name">David</span>
        <img class="chevron" src="../assets/ic_chevron.png" alt="">
    </div>
</template>

<style scoped>
#profile {
    border-radius: 12px;
    border: 1px solid rgba(238, 255, 243, 0.04);
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-right: 8px;
    width: max-content;
}

.profile-name {
    display: none;
}

#profile-pic {
    border-radius: 12px;
    width: 36px;
    aspect-ratio: 1 / 1;
    margin-right: 6px;
}

#profile .chevron {
    width: 15.5px;
    aspect-ratio: 1 / 1;
}

@media (min-width: 768px) {
    #profile {
        padding-right: 12px;
    }

    #profile-pic {
        width: 56px;
        margin-right: 25px;
    }

    #profile .chevron {
        width: 24px;
    }
}

@media (min-width: 992px) {
    .profile-name {
        display: block;
        margin-right: 18px;
    }
}
</style>
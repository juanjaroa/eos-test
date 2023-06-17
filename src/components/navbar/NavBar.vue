<script setup>
import NavMenu from './navbar-items/NavMenu.vue';
import SearchField from './navbar-items/SearchField.vue';
import SettingsButton from './navbar-items/SettingsButton.vue'
import NotificationButtons from './navbar-items/NotificationButtons.vue'
import ProfileMenu from './navbar-items/ProfileMenu.vue';
</script>

<template>
    <header>
        <div class="left-items">
            <NavMenu />
            <img id="logo" src="./assets/logo.png" alt="">
        </div>
        <div class="center-items">
            <SearchField />
            <SettingsButton />
        </div>
        <div class="right-items">
            <NotificationButtons />
            <div class="vertical-divider"></div>
            <ProfileMenu />
        </div>
    </header>
</template>

<style>
header {
    padding: 13px 16px 14px 9px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 1rem;
}

.left-items {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 4px;
    width: auto;
}

#logo {
    width: 45px;
    height: auto;
}

.center-items {
    display: none;
    align-items: center;
    gap: 20px;
}



button {
    width: 36.5px;
    aspect-ratio: 1 / 1;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #2F363D;
    border-radius: 12px;
    position: relative;
}

button>.icon {
    width: 18px;
    height: auto;
}

button .badge {
    width: 10.5px;
    aspect-ratio: 1 / 1;
    background: #D9B75F;
    border-radius: 100%;
    position: absolute;
    top: -2px;
    right: -2px;
}

.right-items {
    display: flex;
    gap: 16px;
    align-items: stretch;
    margin-left: auto;
}

.vertical-divider {
    display: none;
    width: 1px;
    border-radius: 8px;
    background: rgba(246, 246, 246, 0.03);
}

@media (min-width: 567px) {


    .left-items {
        gap: 15px;
    }

    .vertical-divider {
        display: block;
    }

}

@media (min-width: 768px) {
    .center-items {
        display: flex;
        margin-left: 5vw;
        margin-right: auto;
    }


}

@media (min-width: 992px) {
    header {
        padding: 32px 43px 32px 54px;
    }
}

@media (min-width: 1200px) {
    #logo {
        width: 70px;
    }
}

@media (min-width: 1400px) {
    #logo {
        width: 84px;
    }

    button {
        width: 56px;
    }

    button>.icon {
        width: 28px;
    }

    button .badge {
        width: 16px;
        top: -3px;
        right: -3px;
    }

    .right-items {
        gap: 3vw;
    }
}
</style>
<script setup>
import { RouterView, RouterLink } from 'vue-router'
</script>

<template>
    <nav class="navbar is-dark" role="navigation">
        <div class="navbar-brand">
            <span class="navbar-item has-text-weight-bold">🎨 Colour Showcase</span>
        </div>

        <div class="navbar-menu is-active">
            <div class="navbar-start">
                <RouterLink class="navbar-item" to="/">Red</RouterLink>
                <RouterLink class="navbar-item" to="/blue">Blue</RouterLink>
                <RouterLink class="navbar-item" to="/green">Green</RouterLink>
            </div>
        </div>
    </nav>

    <RouterView />
</template>

<style scoped>
.navbar {
    position: sticky;
    top: 0;
    z-index: 10;
}
</style>
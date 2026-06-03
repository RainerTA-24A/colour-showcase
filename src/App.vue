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
                <RouterLink class="navbar-item" active-class="is-active" to="/">Red</RouterLink>
                <RouterLink class="navbar-item" active-class="is-active" to="/blue">Blue</RouterLink>
                <RouterLink class="navbar-item" active-class="is-active" to="/green">Green</RouterLink>
                <RouterLink class="navbar-item" active-class="is-active" to="/yellow">Yellow</RouterLink>
            </div>
        </div>
    </nav>

    <RouterView v-slot="{ Component }">
        <Transition name="fade" mode="out-in">
            <component :is="Component" />
        </Transition>
    </RouterView>
</template>

<style scoped>
.navbar {
    position: sticky;
    top: 0;
    z-index: 10;
}
</style>
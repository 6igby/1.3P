<script setup>
    import { RouterLink } from "vue-router";
</script>

<template>
    <header>
        <nav class="container">
            <div class="port">
                <img src="../assets/briefcase.png" alt="">
                <h1>Portfolio</h1>
            </div>
            <ul class="nav-routes">
                <router-link to="/">Portfolio</router-link>
                <router-link to="/contact">Contact</router-link>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @import url(../assets/MyPortfolio.css);
</style>


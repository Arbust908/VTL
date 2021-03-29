<template>
    <div class="app">
        <Navbar />
        <router-view></router-view>
    </div>
</template>

<script>
import "./Styles/app.sass";

export default {
    name: "app",
    components: {
        Navbar: () => import("./Components/Navbar.vue"),
    },
};
</script>

<template>
    <div class="home">
        <h1>{{ count }}</h1>
        <button
            class="btn font-bold uppercase text-blue-500 hover:text-red-400"
            @click="$store.commit('INCREMENT')"
        >
            Incremantar
        </button>
    </div>
</template>

<script>
import { mapState } from "vuex";

export default {
    name: "home",
    computed: {
        ...mapState({
            count: state => state.count
        })
    }
};
</script>

<style lang="sass" scoped>
.home
    @apply h-full p-8
</style>

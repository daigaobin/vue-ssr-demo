<template>
    <div>
        <h2>News Index Page</h2>
        <ul>
            <li>
                <nuxt-link to="/">HOME</nuxt-link>
            </li>
        </ul>

        <ul>
            <li>
                <nuxt-link to="/news/123">123</nuxt-link>
            </li>
        </ul>

        <ul>
            <li>
                <nuxt-link to="/news/DGB">DGB12</nuxt-link>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'News',
        data () {
            return {}
        },
        created(){

        },
        methods: {},
        components: {},
        watch: {}
    }
</script>

<style scoped>

</style>

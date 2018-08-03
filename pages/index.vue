<template>
    <div>
        <div>
            <ul>
                <li>
                    <nuxt-link to="/">HOME</nuxt-link>
                </li>
                <li>
                    <nuxt-link to="/about">ABOUT</nuxt-link>
                </li>
                <li>
                    <!--<nuxt-link to="/news">NEWS</nuxt-link>-->
                    <nuxt-link :to="{name:'news', params:{id:888}}">NEWS</nuxt-link>
                </li>
            </ul>
        </div>

        <section class="container">
            <div>
                <app-logo/>
                <h1 class="title">
                    nuxt
                </h1>
                <h2 class="subtitle">
                    this is nuxt demo
                </h2>
                <div class="links">
                    <a
                            href="https://nuxtjs.org/"
                            target="_blank"
                            class="button--green">Documentation</a>
                    <a
                            href="https://github.com/nuxt/nuxt.js"
                            target="_blank"
                            class="button--grey">GitHub</a>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    import AppLogo from '~/components/AppLogo.vue'

    export default {
        components: {
            AppLogo
        }
    }
</script>

<style>
    .container {
        min-height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    .title {
        font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
        display: block;
        font-weight: 300;
        font-size: 100px;
        color: #35495e;
        letter-spacing: 1px;
    }

    .subtitle {
        font-weight: 300;
        font-size: 42px;
        color: #526488;
        word-spacing: 5px;
        padding-bottom: 15px;
    }

    .links {
        padding-top: 15px;
    }
</style>

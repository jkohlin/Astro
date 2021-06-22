<template>
    <div>
        <h2>This is a {{variable}} component</h2>
        <p>I just imported it into the astro page. It's as easy as: <pre>import VueComp from '../components/VueComp.vue';</pre></p>
        <p>here's a prop from the astro page:  {{fromAstro}}</p>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                variable: 'vue',
            }
        },
        props: {
            fromAstro: {
                type: String,
            },
        },
    }
</script>

<style lang="scss" scoped>
    h2 {
        color:white;
        background-color:red;
    }
</style>
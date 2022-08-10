<template>
    <div>
        <p>{{ num_friends }}</p>
        <p>{{ logged_in }}</p>
        <p v-for="tweet in tweets" :key="tweet">
             {{ tweet }}
        </p>

    </div>
</template>

<script>
    export default {
        mounted () {
            this.show_info();
        },

        methods: {
            show_info() {
                
            }
        },

        data() {
            return {
                tweets: [`01_tweet`, `02_tweet`, `03_tweet`],
                num_friends : 10,
                logged_in: true
            }
        },
    }
</script>

<style scoped>

</style>
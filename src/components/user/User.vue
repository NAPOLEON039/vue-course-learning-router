<template>
    <div>
        <h1>The User page</h1>
        <hr>
        <p>Loaded route: {{id}}</p>
        <button class="btn btn-info" @click="goToHome()">Go to Home page</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            id: this.$route.params.id
        }
    },
    watch: {
        $route(to, from) {
            this.id = to.params.id;
        }
    },
    methods: {
        goToHome() {
            this.$router.push('/');
        }
    }
}
</script>


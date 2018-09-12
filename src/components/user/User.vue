<template>
    <div>
        <h1>The User page</h1>
        <hr>
        <button class="btn btn-info" @click="goToHome()">Go to Home page</button>
        <hr>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    methods: {
        goToHome() {
            this.$router.push('/');
        }
    },
    created() {
        console.log(this.$route.path);
    }
}
</script>


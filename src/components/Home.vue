<template>
    <div id="home-page">
        <h1>The Home Page</h1>
        <hr>
        <p>Some welcoming text</p>
    </div>
</template>

<script>
export default {
    created() {
        console.log(this.$route.path);
    }
}
</script>

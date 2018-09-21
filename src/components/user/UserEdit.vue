<template>
    <div>
        <h3>Edit user information</h3>
        <hr>
        <router-link :to="'/user/' + $route.params.id" class="btn btn-primary">Back</router-link>
        <hr>
        <button class="btn btn-success" @click="confirmed = true">Confirm leaving</button>
        <div style="height: 700px;"></div>
        <p id="extra">Some extra info about user</p>
    </div>
</template>


<script>
export default {
    data() {
        return {
            confirmed: false
        }
    },
    beforeRouteLeave(to, from, next) {
        if (this.confirmed) {
            next();
        } else {
            next(confirm('Are you sure about this?'))
        }
    }
}
</script>

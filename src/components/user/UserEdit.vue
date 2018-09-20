<template>
    <div>
        <h3>Edit user information</h3>
        <hr>
        <router-link :to="'/user/' + $route.params.id" class="btn btn-primary">Back</router-link>
        <div style="height: 700px;"></div>
        <p id="extra">Some extra info about user</p>
    </div>
</template>

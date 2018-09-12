<template>
    <div id="user-detail">
        <h3>Some user details</h3>
        <p>User loaded has ID: {{$route.params.id}}</p>
        <hr>
        <router-link to="/user" class="btn btn-primary">Back</router-link>
    </div>
</template>

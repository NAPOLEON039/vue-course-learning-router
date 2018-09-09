<template>
    <ul class="nav nav-pills">
        <router-link to="/" tag="li" class="nav-item"><a class="nav-link" :class="{active: this.$route.path == '/'}">Home</a></router-link>
        <router-link to="/user" tag="li" class="nav-item"><a class="nav-link" :class="{active: this.$route.path == '/user'}">User</a></router-link>
    </ul>
</template>

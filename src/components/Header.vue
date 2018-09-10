<template>
    <ul class="nav nav-pills">
        <router-link to="/" tag="li" class="nav-item"><a class="nav-link" :class="{active: this.$route.path == '/'}">Home</a></router-link>
        <router-link to="/user/1" tag="li" class="nav-item"><a class="nav-link" :class="{active: this.$route.path == '/user/1'}">User 1</a></router-link>
        <router-link to="/user/2" tag="li" class="nav-item"><a class="nav-link" :class="{active: this.$route.path == '/user/2'}">User 2</a></router-link>
    </ul>
</template>

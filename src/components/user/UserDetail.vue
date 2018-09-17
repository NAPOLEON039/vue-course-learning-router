<template>
    <div id="user-detail">
        <h3>Some user details</h3>
        <p>User loaded has ID: {{$route.params.id}}</p>
        <hr>
        <router-link to="/user" class="btn btn-primary">Back</router-link>
        <router-link 
            class="btn btn-primary" 
            tag="button" 
            :to="{name: 'userEdit', params: {id: $route.params.id}, query: {locale: 'en'}}"> Edit User
        </router-link>
    </div>
</template>

<template>
    <UserCard v-for="user of users" :key="user.id" :user="user.name" :username="user.username"
        :email="user.email"></UserCard>
</template>


<script>
    import UserCard from './UserCard.vue';

    export default {
        components: {
            UserCard
        },
        data() {
            return {
                users: []
            }
        },
        async created() {
            const response = await fetch('https://jsonplaceholder.typicode.com/users')
            const result = await response.json();
            this.users = result
        }
    }
</script>

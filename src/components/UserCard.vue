<template>
    <div class="user-card">
        <div class="photo">
            <img src="https://picsum.photos/100/100" alt="">
        </div>
        <div class="info">
            <p>User: {{ user }}</p>
            <p>
                User Name: {{ username }}
            </p>
            <p>
                Email: {{ email }}
            </p>
        </div>
        <div>
            <button class="btn">Ver perfil</button>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['user', 'username', 'email']
    }
</script>

<style scoped>
    .user-card {
        padding: 20px;
        background: #fff;
        border: #e2e2e2 solid 2px;
        margin: 10px;
        width: 350px;
        border-radius: 20px 0%;
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        justify-content: center;
    }

    .info {
        margin: 5px;
        line-height: 1;
    }

    .photo>img {
        border-radius: 50%;
    }

    .btn {
        border: none;
        padding: 10px;
    }

    .btn:hover {
        cursor: pointer;
    }
</style>

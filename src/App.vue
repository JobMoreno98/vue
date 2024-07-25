<template>
    <contador></contador>
    <div id="contenedor">
        <Users></Users>
    </div>
</template>
<script>
    import contador from '@/components/contador.vue'
    import Users from '@/components/Users.vue'
    export default {
        components: {
            contador,
            Users,
        },
        
    }
</script>

<style>
    #contenedor {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
</style>

<template>
    <div>
        <p>Contador {{ contador }}</p>
        <button @click="incremet()">Aumentar contador</button>
    </div>
</template>
<script>
    export default {
        name: 'Contador',
        data() {
            return {
                contador: 0
            }

        },
        methods: {
            incremet() {
                this.contador++
            }
        }
    }
</script>

<style scoped>
    button{
        border: none;
        color: #e2e2e2;
        color: #000;
        padding: 5px
    }
</style>

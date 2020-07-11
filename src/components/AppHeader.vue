<template>
    <div>
            <button v-show="loggedIn">Logout</button>
<!--            <button @click="loggedIn = !loggedIn">Toggle button</button>-->
    </div>
</template>

<script>
    export default {
        data() {
            return {
                loggedIn: false
            }
        }
    }
</script>

<style scoped>

</style>

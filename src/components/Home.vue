<template>
    <h1>Hello, Welcome to Home</h1>
</template>

<script>
export default {
    name: 'Home-app',
    mounted() {
        let user = localStorage.getItem('user-info');
        if(!user) {
            this.$router.push({ name: 'SignUp' })
        }
        console.warn("mounted");
    }
}
</script>
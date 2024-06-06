<script>
    import axios from "axios";

    export default {
            name: "Repositories",
            data() {
                return {
                    repos: null,
                };
            },
            created: function() {
                axios.get('https://api.github.com/users/Youngie8/repos').then(response)  => {
                    this.repos = response.data
                }
            }
    }
</script>

<template>
    <h1> Vue</h1>
</template>

<style>

</style>
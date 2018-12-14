<template>
    <div>
        <h1>{{title}}</h1>
    </div>
</template>

<script>
    export default {
        name: 'Title',
        props: {
            title: {
                type: String,
                required: true
            }
        }
    }
</script>

<style scoped>

</style>
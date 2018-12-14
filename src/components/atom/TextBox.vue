<template>
    <div>
        <div class='text-content'>{{content}}</div>
    </div>
</template>

<script>
    export default {
        name: 'TextBox',
        props: {
            content: {
                type: String,
                required: true
            }
        }
    }
</script>

<style scoped>

</style>
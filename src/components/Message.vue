<template>
    <p className="message">
        {{ message }}
    </p>
</template>

<script>
export default {
    name: 'Message',
    props: {
        message: String,
    },
}
</script>

<style>
</style>
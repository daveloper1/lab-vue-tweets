<template>
    <span className="timestamp">{{ timestamp }}</span>
</template>

<script>
export default {
    name: 'Timestamp',
    props: {
        timestamp: String,
    },
}
</script>

<style>
</style>
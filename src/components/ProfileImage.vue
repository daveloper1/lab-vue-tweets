<template>
    <img :src="image" className="profile" alt="profile" />
  
</template>

<script>
export default {
   name: 'ProfileImage',
    props: {
        image: String,
    },
}
</script>

<style>

</style>
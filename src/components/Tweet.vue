<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image"></ProfileImage>

    <div className="body">
      <div className="top">
        <User :userData="tweet.user"></User>
        <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>
      
      <Message :message="tweet.message"></Message>
      <Actions></Actions>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>

import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import ProfileImage from './ProfileImage.vue';
import Actions from './Actions.vue';


export default {
  name: 'Tweet',
  props: {
    tweet: {
      type: Object,
      required: true
    },
  },
  components: { User, Timestamp, Message, ProfileImage, Actions }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>

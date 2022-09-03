<template>
  <div className="tweet">
    <ProfileImage :image="props.tweet.user.image" />

    <div className="body">
      <div className="top">
        <User :userData="props.tweet.user" />
        <Timestamp :time="props.tweet.timestamp" />.
      </div>

      <Message :message="props.tweet.message" />
      <Actions />
      
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import ProfileImage from '../components/ProfileImage.vue'
import User from '../components/User.vue'
import Timestamp from '../components/Timestamp.vue'
import Message from '../components/Message.vue'
import Actions from '../components/Actions.vue'

const props = defineProps({
  tweet: Object,
})

</script>

<style scoped>
a {
  color: #42b983;
}
</style>

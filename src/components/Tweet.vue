<script setup>
defineProps({
  userName: String,
  userImage: String,
  userHandle: String,
  message: String,
  timestamp: String,
})

import ActionComponent from './ActionComponent.vue';
import MessageComponent from './MessageComponent.vue';
import ProfileImage from './ProfileImage.vue';
import TimeStamp from './TimeStamp.vue';
import UserComponent from './UserComponent.vue';
  
</script>


<template>
 <div class="tweet">
    <ProfileImage :userImage ="userImage"></ProfileImage>
    <div class="body">
      <div class="top">
          <UserComponent :userName = "userName"></UserComponent>
          <TimeStamp :timestamp = timestamp></TimeStamp>
      </div>
      <MessageComponent :message ="message"></MessageComponent>
      <div class="actions">
        <ActionComponent></ActionComponent>
      </div>
    </div>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>
defineProps({
  userName: String,
  userImage: String,
  userHandle: String,
  message: String,
  timestamp: String,
})
</script>


<template>
  <div class="tweet">
    <img :src="userImage" class="profile" :alt="userHandle" />
    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ userName }}</span>
          <span class="handle">{{ userHandle }}</span>
        </span>
        <span class="timestamp">{{ timestamp }}</span>
      </div>
      <p class="message">{{ message }}</p>
      <div class="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

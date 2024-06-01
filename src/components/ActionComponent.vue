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
<div class="actions">
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
        <i class="fas fa-ellipsis-h"></i>
      </div>
</template>

<style>

.actions {
    padding: 5px 5px;
    width: 360px;
    display: flex;
    justify-content: space-between;
    color: #536471;
  }
</style>
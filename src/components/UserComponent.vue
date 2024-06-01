<script setup>
defineProps({
  userName: String,
  userHandle: String,
})
</script>

<template>
  <span class="user">
    <span class="name">{{ userName }} </span>
    <span class="handle">{{ userHandle }}</span>
  </span>


</template>

<style>
.name {
  font-weight: bold;
  margin-bottom: 0.5em;
  margin-right: 0.3em;
}

.handle {
  color: #536471;
  margin-left: 3px;
  margin-right: 3px;
}
</style>

<script setup>
defineProps({
  message: String,
})
</script>

<template>

<p class="message">{{ message }}</p>

</template>

<style>
 .message {
    text-align: left;
    font-stretch: 100%;
    font-weight: 400;
    line-height: 1.6rem;
    overflow-wrap: break-word;
    white-space: pre-wrap;
  }
</style>
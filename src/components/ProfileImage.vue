<script setup>
defineProps({
  userImage: String,
})

</script>

<template>

 
    <img :src="userImage" class="profile" :alt="userHandle" />
 



</template>

<style>

  .tweet {
    margin: 0 auto;
    min-width: 480px;
    max-width: 640px;
    min-height: 80px;
    padding: 10px;
    border: 1px solid #ccc;
    display: flex;
    font-size: 1.1rem;
    line-height: 18px;
  }

  .profile {
    width: 50px;
    height: 50px;
    border-radius: 50px;
    margin-right: 10px;
  }
  

</style>
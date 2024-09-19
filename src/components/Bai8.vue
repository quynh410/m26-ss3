<template>
  <div>
    <a href="https://www.google.com" @click="checkLink">Click me</a>
  </div>
</template>

<script setup>
const checkLink = (event) => {
  const link = event.target.href;
  
  if (!link.startsWith(' http://www.google.com')) {
    event.preventDefault(); 
    alert('Đường dẫn không hợp lệ.');
  }
};
</script>

<style>
</style>

<template>
  <div>
    <button @click="handleClick('Rikkei Academy')">Get param</button>
  </div>
</template>

<script setup>
function handleClick(param) {
  console.log(param); 
}
</script>

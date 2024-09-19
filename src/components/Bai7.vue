<template>
  <div>
    <form @submit.prevent="handleSubmit">
      <input type="text" />
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script setup>
const handleSubmit =()=> {
  console.log('Form submission prevented!');
}
</script>

<style></style>

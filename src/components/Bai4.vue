<template>
  <div>
    <div
      v-bind:class="{ active: isActive }"
      :style="{ backgroundColor: backgroundColor }"
    >
      Block
    </div>
  </div>
</template>

<script setup>
const isActive = true;
const backgroundColor = "#0000FF";
</script>

<style>
.active {
  color: #fff; 

}
</style>

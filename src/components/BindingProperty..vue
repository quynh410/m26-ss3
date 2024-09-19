<script setup>
const url =
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS2mDpMHhQYm5lytlAIdf57Y7COk0r6O03RBg&usqp=CAU";
const isDisabled = false;
const inpDisabled = true;
const divAttributes = {
  id: "container",
  class: "myClass",
};
const divStyle = {
  id: "paragraph",
  area: "paragraph",
};
const isTextRed = true;
</script>

<template>
  <div>
    <img v-bind:src="url" alt="" />
    <!-- <img :src="url" alt="" />   -->
    <button v:bind:disabled="isDisabled">Click me</button> <br />
    <input type="text" :disabled="inpDisabled" />
    <div v-bind="divAttributes">Container</div>
    <!-- binding 2 thuoc tinh id:"paragraph" , area="paragraph" -->
    <p v-bind="divStyle">Noi dung</p>
    <!-- v-bind cho class va style -->
    <div v-bind:class="{ textRed: isTextRed }">Hello world</div>
  </div>
</template>

<style>
.textRed {
  color: red;
}
</style>

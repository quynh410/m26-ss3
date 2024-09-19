<script setup>
const handleClick = () => {
  console.log("Clicked");
};
const handleDelete = (id) => {
  console.log("ID : ", id);
};
const handleGetEvent = (event) => {
  console.log("Event Info : ", event);
};
const handleSubmit = ()=>{
    alert("Submit ngan lai hanh dong load lai trang")
}
// duoc kich hoat khi nguoi dung nhan vao nut dong form hoac nhan phim esc 
const handleCloseForm = ()=>{
    alert("Form da dong")
}
</script>

<template>
  <div>
    <button v-on:click="handleClick">Click me</button>
    <button v-on:click="handleDelete(1)">Delete</button>
    <button @click="handleGetEvent">Event Info</button>
    <!-- Cú pháp rút ngắn -->
    <!-- <button @click="handleClick">Click</button> -->
    <form @submit.prevent="handleSubmit">
        <button type="submit">Submit</button>
    </form>
    <!--  -->
    <button @keydown.esc="handleCloseForm">Dong form</button>
  </div>
</template>

<style></style>

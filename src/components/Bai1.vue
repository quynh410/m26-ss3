<script setup>
const url =
  "https://p16-sign-sg.tiktokcdn.com/aweme/720x720/tos-alisg-avt-0068/7f2366302a6a5fc11d69fc079eaf2f19.jpeg?lk3s=a5d48078&nonce=71401&refresh_token=b253c05dc1cadb379d8815bb87875006&x-expires=1726902000&x-signature=pZghB4ohO%2BMFQb1JtjTtyk%2FyhPM%3D&shp=a5d48078&shcp=81f88b70";
const image = true;


</script>

<template>
  <div>
    <img :class="{ img: image }" :src="url" alt="" />
  </div>
</template>

<style>
.img {
  width: 200px;
  height: 200px;
  object-fit: cover;
  border-radius: 5px;
}
</style>

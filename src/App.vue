<script setup>
import { ref } from "vue";

//setup 필수!!
//01.데이터 바운딩작업
const count = ref(0);
//데이터 바운딩작업을 한다면 ref객체를 쓴다.
</script>

<template>
  <div @click="count++" class="btn-cnt">Count is {{ count }}</div>
  <button @click="count = 0">Count Reset</button>
</template>
<style>
.btn-cnt {
  width: 100px;
  height: 100px;
  line-height: 100px;
  background-color: blue;
  color: aliceblue;
  border: 0;
}
button {
  width: 100px;
  height: 100px;
  line-height: 100px;
  background-color: rgb(250, 27, 94);
  color: aliceblue;
  border: 0;
}
</style>

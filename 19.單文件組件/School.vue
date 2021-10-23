<template>
  <div class="demo">
    <h2>學校名稱: {{ name }}</h2>
    <h2>學校地址: {{ address }}</h2>
    <button @click="showName">點我提示學校名</button>
  </div>
</template>

<script>
//組件交互相關的代碼(數據、方法等等) js需用es6 暴露
export default {  //直接省略Vue.extend
  name: "School",
  data() {
    return {
      name: "台東高中",
      address: "台東市",
    };
  },
  methods: {
    showName() {
      alert(this.name);
    },
  },
};
// export {school}  //統一暴露 import {???} from ???
// export default school //默認暴露  import ??? from ??? (vue通常這樣寫，因為只有一個)
</script>

<style>
/* 組件的樣式 */
.demo {
  background-color: orange;
}
</style>
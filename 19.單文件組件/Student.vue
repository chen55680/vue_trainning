<template>
  <div class="demo">
    <h2>學生姓名: {{ name }}</h2>
    <h2>學生年齡: {{ age }}</h2>
    <button @click="showName">點我提示學生姓名</button>
  </div>
</template>

<script>
//組件交互相關的代碼(數據、方法等等) js需用es6 暴露
export default {  //直接省略Vue.extend
  name: "Student",
  data() {
    return {
      name: "張三",
      age: 18,
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

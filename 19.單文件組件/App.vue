<template>
  <div>
    <school></school>
    <student></student>
  </div>
</template>

<script>
//引入組件
import School from "./School.vue";
import Student from "./Student.vue";

export default {
  name: "App",
  template:`<App></App>`,
  components: {
    School,
    Student,
  },
};
</script>

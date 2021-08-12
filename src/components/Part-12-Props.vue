<template>
  <div>
    <h1>Props Concept</h1>
    <Student :name="name" />
    <Teacher :name="name" />
  </div>
</template>
<script>
import Student from "./Student.vue";
import Teacher from "./Teacher.vue";
export default {
  name: "Props",
  data(){
      return {
        name:'Anil'
      }
  },
  components: { Student, Teacher },
};
</script>
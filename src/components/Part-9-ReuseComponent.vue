<template>
  <div>
    <h2>Reuse component</h2>
    <ul>
      <li v-for="item in users" :key="item">
        <User :data="item" :getData="getData"/>
      </li>
    </ul>
  </div>
</template>

<script>
import User from "./User.vue";
export default {
  name: "ReuserComponent",
  components: {
    User,
  },
  methods: {
      getData(name){
          alert(name);          
      },
  },
  data() {
    return {
      users: [
        {
          name: "anil",
          email: "anil@test.com",
        },
        {
          name: "deep",
          email: "deep@test.com",
        },
      ],
    };
  },
}
</script>
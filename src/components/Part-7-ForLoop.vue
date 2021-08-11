<template>
    <div>
        <h1>For Loop</h1>
        <ul >
            <li v-for="item in technology" :key="item">{{item}}</li>
            
        </ul>
        <br/>
        <ul>
            <li v-for="item in user" :key="item">My name is : "{{item.name}}" & email is : "{{item.email}}"</li>
        </ul>
    </div>
</template>

<script>
export default {
    name:'ForLoop',
    data(){
       return{
          technology:['Java','PHP','HTML','CSS'],
          user:[{
              name:"anil",
              email:"anil.vaja@zoodmall.com",
              },{
              name:"deep",
              email:"dip.vaja@zoodmall.com",
              },{
              name:"shiv",
              email:"shiv.vaja@zoodmall.com",
              }
          ]
       }
    },
    methods: {
      
    },
}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
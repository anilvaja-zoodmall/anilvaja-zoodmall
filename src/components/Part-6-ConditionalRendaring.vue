<template>
    <div>
        <h1>Conditional Rendering If , else if, else</h1>
        <button v-on:click="show=!show" >Toggle</button>
        <h3 v-if="show">Show</h3>
        <h4 v-if="!hide">hide</h4>  <br/>  <br/>  <br/>
        
        <h3 v-if="show">if</h3>
        <h4 v-else>else</h4>
    </div>
</template>

<script>
export default {
    name:'ConditionalRendaring',
    data(){
       return{
           show:true,
           hide:false,
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
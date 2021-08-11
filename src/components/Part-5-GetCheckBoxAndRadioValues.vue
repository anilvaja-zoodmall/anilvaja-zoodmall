<template>
    <div>
        <h1>Checkbox & radio box values</h1>
        <label for="java">java</label>
        <input type="checkbox" value="java" id="java" v-model="technology" /> &nbsp;&nbsp;
        <label for="php">php</label>
        <input type="checkbox" value="php" id="php" v-model="technology"  />&nbsp;&nbsp;
        <label for="Node">Node</label>
        <input type="checkbox" value="Node" id="Node" v-model="technology"  />&nbsp;&nbsp;
        <label for="javascript">javascript</label>
        <input type="checkbox" value="javascript" id="javascript" v-model="technology"  />
        <h4>selected technology : {{technology}}</h4>
        <br />
        <br />
        <br />
        <h3>Who I am</h3>
        <label for="student">student</label>
        <input type="radio" value="student" id="student" name="profession" v-model="who"  />&nbsp;&nbsp;
        <label for="developer">developer</label>
        <input type="radio" value="developer" id="developer" name="profession" v-model="who"  />&nbsp;&nbsp;
        <h4>I am a {{who}}</h4>
        




<br/><br/><br/>


    </div>
</template>

<script>
export default {
    name:'GetCheckBoxAndRadioValues',
    data(){
       return{
           technology:[],
           who:[],
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
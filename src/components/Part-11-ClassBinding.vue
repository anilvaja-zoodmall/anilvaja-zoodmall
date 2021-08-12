<template>
    <div :class="applyStyles">
            <h2>Class Bindings</h2>
    </div>    
    <button v-on:click="colorFull=!colorFull,err=!err">Click to change color</button>
</template>

<script>
export default {
    name:'ClassBinding',
    data(){
        return {
            colorFull:true,
            err:true,
            other:true
        }
    },
    computed:{
        applyStyles(){
            return{
                green:this.colorFull,
                err:this.err,
                other:this.other

            }
        },
    }
}
</script>
<style>
 .green
 {
     background-color: green;

 }
 .err
{
    color:red;
}
.other
{
    font-size: 50px;
}
</style>
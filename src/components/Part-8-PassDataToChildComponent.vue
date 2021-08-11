<template>
    <div>
        <h1>Pass Data To ChildComponent</h1>
        <Child name="Anil Vaja" :user="user"  :getData="getData"/>
    </div>
</template>
<script>
import Child from './Child.vue'
export default {
    name:"PassDataToChildComponent",
    components:{Child},
    data(){
        return{
            user:{name:'Deep',email:'deep.vaja@gmail.com'}
        }
    },
    methods: {
        getData() {
            console.warn('Parent function called')
        },
    },
}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
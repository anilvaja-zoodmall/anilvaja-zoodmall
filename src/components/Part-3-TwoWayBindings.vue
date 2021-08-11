<template>
    <div>
        <input type="number" v-model="count"/>
        <h3>Square : {{count*count}}</h3>
        <h3>sqrt : {{Math.sqrt(count)}}</h3>W
        
    </div>
</template>

<script>
export default {
    name:'TwoWayBindings',
    data(){
        return {
            count:4
        }
    }
}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
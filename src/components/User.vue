<template >
    <div class="user">
        <h3>{{data.name}}</h3>
        <h3>{{data.email}}</h3>
        <button v-on:click="getData(data.name)">Click here</button>
    </div>
</template>

<script>
export default {
    name:'User',
    props:{
        data:Object,
        getData:Function
    }
}
</script>
<style scoped>
.user{
    align-items: center;
    background-color: gray;
    color:white;
    padding:10px;
    border-bottom: 1px solid;
    width:200px ;
}
</style>
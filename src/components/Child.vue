<template>
    <div>
        <h1>This is Child</h1> 
        <div>{{name}}</div>
        <div>{{user.name}}</div>
        <div>{{user.email}}</div>
        <button v-on:click="getData()">Click Here</button>
    </div>
</template>
<script>
export default {
    name:"child",
    props: {
            name:  String,
            user: Object,
            getData: Function,
        }
}
</script>
<template>
    <div>
        <input type="text" placeholder="Enter username" v-model="email" />
        <br/>
        <br/>
        <input type="password" placeholder="Enter Password" v-model="password"/>
        <br/>
        <br/>
        <button v-on:click="getData()" type="button">get Data</button>
    </div>
</template>

<script>
export default {
    name:'GetInputValues',
    data(){
        return {
            email:null,
            password:null
        }
    },
    methods: {
        getData() {
            console.warn('Values : ' ,this.email, this.password)
        },
    },
}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
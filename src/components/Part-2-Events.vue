<template>
    <div>
        <h1 v-on:mousemove="getConsole()">Home Component</h1>
        <button v-on:click="getData('Button1 Clicked')">Button 1 </button><br/>
        <button v-on:click="test()">Button 2 </button><br/>
        <button v-on:dblclick="doubleClickData('Button double  Clicked')">Button 3 > doubleClick </button><br/>
        <h2>Count : {{count}}</h2>
        <button v-on:click="countIncrese()">Increse the count</button><br/>
        
    </div>
</template>
<script>
export default {
    name:'Home',
    data(){
        return  {
            count:0
        }
    },
    methods: {
        countIncrese()
        {
            this.count+=1
        },
        getData(data) {
            alert(data);
        },
        doubleClickData(data){
            alert(data);

        },
        test() {
            alert('Button 2 clicked');
        },
        getConsole(){
            console.warn('Mouse move called');
        }
    },
}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
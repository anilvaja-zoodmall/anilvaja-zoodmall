<template>
    <div>
        <input type="text" v-modal="count"/>
        <h3>Count {{count}}</h3>
    </div>
</template>

<script>
export default {
    name:'TwoWayBindings',
    data(){
        return {
            count:0
        }
    }

}
</script>
<style scoped>
    h1{
        color:orange
    }
</style>
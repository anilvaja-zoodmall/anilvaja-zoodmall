<template>
    <div>
        <h1>Teacher name is {{name}}</h1>

    </div>    
</template>
<script>
export default {
    name:'Teacher',
    props:{
        name:String
    }
}
</script>
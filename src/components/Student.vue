<template>
    <div>
        <h1>Student name is {{name}}</h1>
    </div>    
</template>
<script>
export default {
    name:'Student',
    props:{
        name:String
    }


}
</script>
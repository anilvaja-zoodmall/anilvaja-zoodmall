<template>
    <div>
        
        <h3>Home component</h3>
        <h3>{{10 + 10}}</h3>
        <h3>"Hello".length  {{"Hello".length}}</h3>
        <h3>Email: <span>{{email}}</span></h3>
        <h3>Mobile: <span>{{mobile}}</span></h3>
        <h3>Mobile: <span>{{mobile==8888}}</span></h3>
        <h3>Name: <span>{{getName("Anil Vaja")}}</span></h3>
        <h3>Full Name: <span>{{getData().firstName+ " "+getData().lastName}}</span></h3>
        <h3>New E mail: <span>{{getData().email}}</span></h3>
    </div>
</template>
<script>
export default{
    name:'Home2',
    data()
    {
        return {
            email:'anil.vaja@zoodmall.com',
            mobile:99999,
            getName:function($a){
                return $a
            }
        }
    },
    methods:{
        getData()
        {
            return {
                firstName:'Anil',
                lastName:'Anil',
                email:'Anil.vaja111@zoodmall.com',
                mobile:9510474740
            }
        }
    }
}
</script>

<style scoped>
    h3{
        color:orange;
    }
    span{
        color:violet
    }
</style>
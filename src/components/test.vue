<template>
    <h2 class="red">test..{{msg}}</h2>    
</template>

<script>
export default {
    name:"test",
    props:{
        msg:{
            type:String,
            default:"test msg"
        }
    },
    methods:{       //注意vue实例对象的每一个属性需要有冒号

    },
    data(){
        return{
        }
    },
}
</script>


<style scoped>
    .red{
        color: red;

    }
</style>
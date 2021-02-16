<template>
我是一个用户组件
<ul>
    <li v-for="(item,index) in list" :key=index>
        {{item}}
    </li>
</ul>
 
</template>

<script>

export default {
    data(){
        return {
           list:[]
        };
    },
    mounted(){
        for(var i = 0;i < 10;i++){
            this.list.push(`我是第${i}条数据`); //ES6写法

        }
    }
    
 
}
</script>

<style>

</style>

<template>
<h2>{{msg}}</h2>
<hr>
<home/>
<hr>
<User/>
 
</template>

<script>

//1.引入组件
import Home from './components/Home';
import User from './components/User';
export default {
    data(){
        return {
            msg:"app根组件"
        };
    },
    components:{  //2.挂在组件
        Home,
        User
    }

 
}
</script>

<style>
h2{
    text-align: center;
}

</style>

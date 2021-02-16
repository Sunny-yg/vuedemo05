<template>
<h5>{{title}}</h5>
<button @click="getTitle()">获取Home组件的title</button>
<Header/>
</template>
<script>
import Header from './Header';
export default {
    data(){
        return{
            title:"首页组件"
        }
    },
    methods:{
        getTitle(){
            alert(this.title);
        }
    },
    components:{
        Header
    }
}

</script>

<style>
h5{
    text-align: center;
}
</style>
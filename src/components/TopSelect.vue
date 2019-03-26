<template>
    <div class="top-select">
        <div class="item-list">
            <ul>
                <li v-for='item in list' :key="item" @click="toThisPages(item)">
                    {{item}}
                </li>
            </ul>
            <span><img src="../assets/topSelect/bar.png"></span>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            msg:'',
            list:['推荐','热点','娱乐','财经','视频','新时代','军事','推荐','热点','娱乐','财经']
        }
    },
    methods:{
        toThisPages(item){    // 去点击的页面
            console.log(item+'=====被点击了');
        }
    }
}
</script>

<style scoped>
.top-select{
    position: relative;
    padding:0 15px;
}
.top-select .item-list{
    width:100%;
    height:40px;
    white-space: nowrap;
    overflow: hidden;
    overflow-x: scroll;
}
.item-list ul{
    padding:0;
    margin:0;
}
.item-list ul li{
    list-style: none;
    line-height: 40px;
    display: inline-block;
    margin:0 10px;
    color:#000;
}
.item-list ul li.active{
    color:red;
}
.top-select span{
    width:32px;
    height: 32px;
    display: block;
    background: #ffffff;
    position: absolute;
    right: 14px;
    top:0;
}
.top-select img{
    width:100%;
    height: 100%;
}
</style>


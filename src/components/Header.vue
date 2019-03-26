<template>
    <div class="header">
        <div class="top-bar">
            <div class="search">
                <label class="inp-txt" for="input-id">
                    <img src="../assets/header/search.png">
                    <span>{{txt}}</span>
                </label>
                <input type="text" id="input-id" v-model="inpVal" @focus="getFocus" @blur="outBlur">
            </div>
            <div class="photo">
                <img src="../assets/header/photo.png">
                <span>发布</span>
            </div>
        </div>
    </div>
</template>
<script>
export default{
    data(){
        return{
            msg:'top-bar页面',
            txt:'',
            inpVal:'请输入要搜索的内容'
        }
    },
    methods:{
        getFocus(){
            if(this.inpVal == '请输入要搜索的内容'){
                this.inpVal = '';
            }
        },
        outBlur(){
            if(this.inpVal == ''){
                this.inpVal = '请输入要搜索的内容';
            }
        }
    }
}
</script>
<style scoped>
    .header{
        width: 100%;
        height:50px;
        background:#d43d3d;
        padding:0 15px;
        box-sizing: border-box;
    }
    .top-bar{
        display: flex;
    }
    .top-bar .photo{
        flex: 2;
        text-align: center;
    }
    .top-bar .photo span{
        font-size: 12px;
        display: block;
        margin-top: -5px;
        color:#fff;
    }
    .top-bar .search{
        flex:10;
        position: relative;
    }
    .top-bar .inp-txt{
        position: absolute;
        left:5px;
        top:12px;
    }
    .inp-txt img{
        vertical-align: middle;
        width: 24px;
    }
    .top-bar input{
        width:100%;
        height: 30px;
        line-height: 30px;
        border:none;
        outline: none;
        margin-top: 9px;
        border-radius: 5px;
        text-indent: 30px;
    }
</style>

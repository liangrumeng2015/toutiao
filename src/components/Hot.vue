<template>
    <div class="hot-news">
        <ul v-for="item in list">
            <!-- 左右布局 -->
            <li class="item1" v-if="item.img.length == 1">
                <div class="left-txt">
                    <span>{{item.title}}</span>
                    <div class="bottom-part">
                        <div>
                            <img src="../assets/hot/hot.png">
                            <span>{{item.fromPlat}}<i>{{item.commentNum}}评</i></span>
                        </div>
                    </div>
                </div>
                <div class="right-img">
                    <img class="imgW" :src="item.img[0]">
                </div>
            </li>
            <!-- 上下布局 -->
            <li class="item2" v-else>
                <div class="top-txt">
                    {{item.title}}
                </div>
                <div class="img-three">
                    <img :src="item.img[0]">
                    <img :src="item.img[1]">
                    <img :src="item.img[2]">
                </div>
                <div class="bottom-part">
                    <div>
                        <img src="../assets/hot/hot.png">
                        <span>{{item.fromPlat}}<i>{{item.commentNum}}评</i></span>
                    </div>
                    <span></span>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
        data(){
            return{
                msg:'',
                list:[]      // 拿到列表里面的值
            }
        },
        created(){
            this.getData();
        },
        methods:{
            getData(){
                var api = 'https://easy-mock.com/mock/5c9a254c348ab3569aac9ff4/toutiao/hot';
                this.$axios.get(api).then((res)=>{
                    console.log(res);
                    this.list = res.data.data.list;
                }).catch((error)=>{
                    console.log(error);
                })
            }
        }
    }
</script>

<style scoped>
*{
    margin:0;
    padding:0;
    list-style: none;
}
.hot-news{
    padding:0 10px;
}
.item1{
    display:flex;
    padding-bottom:5px;
    margin-bottom:20px;
    border-bottom:1px solid rgba(221, 221, 221, 0.6);
}
.item1 .left-txt{
    flex:8;
}
.item1 .right-img{
    flex:3;
    text-align: right;
}
img.imgW{
    width:100%;
}
.bottom-part img{
    width:16px;
}
.bottom-part span{
    color:#999;
    font-size: 12px;
}
.bottom-part span i{
    font-style: normal;
    margin-left: 5px;
}
.item2{
    border-bottom:1px solid rgba(221, 221, 221, 0.6);
    padding-bottom:5px;
    margin-bottom:20px;
}
.item2 .top-txt{
    line-height: 30px;
}
.img-three{
    font-size:0;
    margin-bottom:5px;
}
.img-three img{
    width:32%;
    margin-right:1%;
}
.img-three img:nth-child(3){
    margin-right:0;
}

</style>




<template>
    <div class="hot-news">
        <ul>
            <!-- 左右布局 -->
            <li class="item1">
                <div class="left-txt">
                    <span>美国唯一的空降部队-陆军第82空降师</span>
                    <div class="bottom-part">
                        <div>
                            <img src="../assets/hot/hot.png">
                            <span>人民日报海外站<i>100评</i></span>
                        </div>
                        <span></span>
                    </div>
                </div>
                <div class="right-img">
                    <img class="imgW" src="https://p3.pstatp.com/list/pgc-image/38cb52aab2b749ab9f9c354480f8c531">
                </div>
            </li>
            <li class="item1">
                <div class="left-txt">
                    <span>美国唯一的空降部队-陆军第82空降师</span>
                    <div class="bottom-part">
                        <div>
                            <img src="../assets/hot/hot.png">
                            <span>人民日报海外站<i>100评</i></span>
                        </div>
                        <span></span>
                    </div>
                </div>
                <div class="right-img">
                    <img class="imgW" src="https://p3.pstatp.com/list/pgc-image/38cb52aab2b749ab9f9c354480f8c531">
                </div>
            </li>
            <!-- 上下布局 -->
            <li class="item2">
                <div class="top-txt">
                    谁说女子不如男！中国第一女司机，24岁轻松开动6万吨航母
                </div>
                <div class="img-three">
                    <img class="imgW" src="https://p3.pstatp.com/list/pgc-image/fb6c1e8a57074998a6fcd09dc43e9237">
                    <img class="imgW" src="https://p3.pstatp.com/list/pgc-image/fb6c1e8a57074998a6fcd09dc43e9237">
                    <img class="imgW" src="https://p3.pstatp.com/list/pgc-image/fb6c1e8a57074998a6fcd09dc43e9237">
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
*{
    margin:0;
    padding:0;
    list-style: none;
}
.hot-news{
    padding:0 15px;
}
.item1{
    display:flex;
    margin-bottom:10px;
}
.item1 .left-txt{
    flex:8;
}
.item1 .right-img{
    flex:4;
    text-align: right;
}
img.imgW{
    width:100px;
    height: 65px;
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
.item2 .top-txt{
    line-height: 30px;
}
.img-three{
    text-align: center;
}

</style>




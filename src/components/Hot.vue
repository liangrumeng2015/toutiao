<template>
    <div class="hot-news">
        <ul>
            <li class="item">
                <div class="left-txt">
                    <span>美国唯一的空降部队-陆军第82空降师</span>
                    <div class="bottom-part">
                        <div>
                            <img src="">
                            <span>人民日报海外站</span>
                        </div>
                        <span></span>
                    </div>
                </div>
                <div class="right-img">
                    <img src="https://p3.pstatp.com/list/pgc-image/38cb52aab2b749ab9f9c354480f8c531">
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
}
.hot-news{
    padding:0 15px;
}
.item{
    display:flex;
}
.item .left-txt{
    flex:8;
}
.item .right-img{
    flex:4;
    text-align: right;
}
.right-img img{
    width:100px;
    height: 65px;
}
</style>


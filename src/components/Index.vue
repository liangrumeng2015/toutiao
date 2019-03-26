<template>
<!-- 推荐页面 -->
    <div class="recommand">
        <v-header></v-header>
        <v-topSelect></v-topSelect>
        <v-hot></v-hot>
        <v-video></v-video>
    </div>
</template>
<script>
import Header from './Header';
import TopSelect from './TopSelect';
import Hot from './Hot';
import Video from './Video';
export default{
    data(){
        return{
            msg:''
        }
    },
    components:{
        'v-header':Header,
        'v-topSelect':TopSelect,
        'v-hot':Hot,
        'v-video':Video
    }
}

</script>
<style scoped>

</style>

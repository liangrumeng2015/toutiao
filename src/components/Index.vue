<template>
<!-- 推荐页面 -->
    <div class="recommand">
        <v-header></v-header>
        <v-topSelect></v-topSelect>
        <v-hot></v-hot>
    </div>
</template>
<script>
import Header from './Header';
import TopSelect from './TopSelect';
import Hot from './Hot';
export default{
    data(){
        return{
            msg:''
        }
    },
    components:{
        'v-header':Header,
        'v-topSelect':TopSelect,
        'v-hot':Hot
    }
}

</script>
<style scoped>

</style>

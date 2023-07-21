<template>
    <div class="index">
        <Header style="margin:0"></Header>
        <Aside></Aside>
        <router-view></router-view>
        <!-- <div class="center">
            <div class="bg">
                <el-button class="button" circle><el-avatar :size="100" :src="circleUrl"></el-avatar></el-button>
                <h1 style="margin-right: 150px; color: black;">小熊软糖杀手</h1>
            </div>

        </div> -->

        <!-- <Footer></Footer> -->

    </div>
</template>

<script>
import Header from "../Header.vue"
import Aside from "../personcenter/Aside.vue"
import Footer from '../Footer.vue'


export default {
    name: 'index',
    data() {
        return {
            circleUrl: require("../../assets/block.png"),//头像图片
        }
    },
    components: {
        Header,
        Aside,
        Footer
    }
};
</script>

<style>
*{
    margin: 0;
    padding: 0;
}
.index {
    width: 100%;
    height: 100%;
    overflow: hidden;
    background: linear-gradient(to bottom, #8da1f8, #fab2f1);
}

.center {
    width: 100%;
    height: 900px;
}

.bg {
    width: 100%;
    height: 100%;
    margin-left: 50px;
    background: url('../../assets/bg.gif');
    /* background-size: cover; */
}


</style>

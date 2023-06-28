<template>
    <div class="index">
        <Header style="margin:0"></Header>
        <Aside></Aside>
        <router-view></router-view>


        <Footer style="margin: 0;padding: 0;"></Footer>

    </div>
</template>

<script>
import Header from "../Header.vue"
import Aside from "../personcenter/Aside.vue"
import Footer from '../Footer.vue'


export default {
    name: 'index',
    components: {
        Header,
        Aside,
        Footer
    }
};
</script>

<style>
.index {
    background-color: rgb(216, 216, 216);
    width: 100%;
    height: 100%;
    overflow: hidden;
}
</style>

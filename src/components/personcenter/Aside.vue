<template>
    <div class="left">
        <el-menu background-color="#545c64" text-color="#ffffff"
                 active-text-color="#ffd04b" class="el-menu-vertical-demo"
                    router>
            <el-menu-item index="/index/menu1"><i class="el-icon-user"></i>用户信息</el-menu-item>
            <el-submenu index="/index/menu2">
                <template slot="title"><i class="el-icon-document"></i><span>笔记整合</span></template>
                <el-menu-item index="/index/menu2">所有</el-menu-item>
                <el-menu-item index="/index/menu2">分类</el-menu-item>
            </el-submenu>
            <!-- <el-menu-item index="/index/menu2"><i class="el-icon-document"></i>笔记整合</el-menu-item> -->
            <el-menu-item index="/index/menu3"><i class="el-icon-setting"></i>个人设置</el-menu-item>
        </el-menu>
    </div>
</template>

<script>
    export default {
        name: "Aside"
    }
</script>

<style scoped>
.left{
    display: flexbox;
    float: left;
    width: 300px;
    height: 900px;
}
    .el-menu-vertical-demo{
        height: 100%;
    }
</style>

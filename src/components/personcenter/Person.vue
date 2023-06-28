<template>
    <div>
        <Header style="margin: 0;"></Header>
        <el-row class="tac">
            <el-col :span="12">
                <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose"
                    background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
                    <el-submenu index="1">
                        <template slot="title">
                            <i class="el-icon-location"></i>
                            <span>个人信息</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="1-1">选项1</el-menu-item>
                            <el-menu-item index="1-2">选项2</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-menu-item index="2">
                        <i class="el-icon-menu"></i>
                        <span slot="title">笔记集合</span>
                    </el-menu-item>
                    <el-menu-item index="4">
                        <i class="el-icon-setting"></i>
                        <span slot="title">个人设置</span>
                    </el-menu-item>
                </el-menu>
            </el-col>
        </el-row>
        <Footer></Footer>
    </div>
</template>

<script>

import Footer from '../Footer.vue'
import Header from '../Header.vue'

export default {
    name: 'Person',
    methods: {
        handleOpen(key, keyPath) {
            console.log(key, keyPath);
        },
        handleClose(key, keyPath) {
            console.log(key, keyPath);
        }
    },
    components: {
        Header, Footer
    }
}
</script>

<style scoped>
.tac{
    margin: 0;
    padding: 0;
    width: 100%;
    height: 800px;
}
.el-menu-vertical-demo{
    width: 300px;
    height: 800px;
}
</style>
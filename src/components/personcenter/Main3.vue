<template>
    <div class="main3">
        <el-card class="box-card">
            <img src="../../assets/block.png" alt="" width="100px" height="100px">
            <el-descriptions class="margin-top" title="带边框列表" :column="3" :size="size" border>
                <template slot="extra">
                    <el-button type="primary" size="small" @click="edit">操作</el-button>
                </template>
                <el-descriptions-item>
                    <template slot="label">
                        <i class="el-icon-user"></i>
                        用户名
                    </template>
                    kooriookami
                </el-descriptions-item>
                <el-descriptions-item>
                    <template slot="label">
                        <i class="el-icon-mobile-phone"></i>
                        手机号
                    </template>
                    18100000000
                </el-descriptions-item>
                <el-descriptions-item>
                    <template slot="label">
                        <i class="el-icon-location-outline"></i>
                        居住地
                    </template>
                    苏州市
                </el-descriptions-item>
                <el-descriptions-item>
                    <template slot="label">
                        <i class="el-icon-tickets"></i>
                        备注
                    </template>
                    <el-tag size="small">学校</el-tag>
                </el-descriptions-item>
                <el-descriptions-item>
                    <template slot="label">
                        <i class="el-icon-office-building"></i>
                        联系地址
                    </template>
                    江苏省苏州市吴中区吴中大道 1188 号
                </el-descriptions-item>
            </el-descriptions>


        </el-card>
    </div>
</template>

<script>
export default {
    name: "Main3",
    methods:{
        edit() {
      this.$refs.dia.open();
    },
    }
}

</script>

<style scoped>
.main3 {
    margin-left: 480px;
    width: 600px;
    height: 800px;


}

.box-card {
    margin-top: 100px;
    width: 930px;
    height: 600px;

}
.margin-top{
    margin-top:20px
}
</style>

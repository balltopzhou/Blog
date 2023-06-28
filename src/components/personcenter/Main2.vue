<template>
    <div class="main2">
        <el-card class="box-card">

       
        <el-table :data="tableData" stripe style="width: 100%">
            <el-table-column prop="date" label="日期" width="180">
            </el-table-column>
            <el-table-column prop="name" label="类别" width="180">
            </el-table-column>
            <el-table-column prop="title" label="标题">
            </el-table-column>
        </el-table>
    </el-card>
    </div>
</template>

<script>
export default {
    name: "Main2",
    data() {
        return {
            tableData: [{
                date: '2016-05-02',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1518 弄'
            }, {
                date: '2016-05-04',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1517 弄'
            }, {
                date: '2016-05-01',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1519 弄'
            }, {
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },{
                date: '2016-05-03',
                name: '王小虎',
                title: '上海市普陀区金沙江路 1516 弄'
            },
        ]
        }
    }
}
</script>

<style scoped>
.main2 {
    margin-left: 400px;
    width: 100%;
    height: 800px;

}
.box-card {
    margin-top: 100px;
    width: 930px;
    height: 600px;

}
</style>

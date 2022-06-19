<template>
  <div class="hello">
    <el-table :data="tableData">
      <el-table-column prop="date" label="日期" width="140"></el-table-column>
      <el-table-column prop="name" label="姓名" width="120"></el-table-column>
      <el-table-column prop="address" label="地址" width="240"></el-table-column>
      <el-table-column prop="none" label="操作"><el-button type="primary" size="default" @click="_blank">编辑</el-button></el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    const item = {
      date: '2016-05-02',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1518 弄'
    }
    return {
      // tableData: Array(5).fill(item)
      tableData : [{date:'2019-09-19',name:'雯笙',address:'河南经贸'}],
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

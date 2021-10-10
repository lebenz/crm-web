<template>
  <div class="app-container">
    <!-- <crudOperation show="" :permission="permission" /> -->
    <el-table ref="table" style="width: 100%;">
      <el-table-column prop="userName" label="id" />
      <el-table-column prop="nickName" label="客户名称" />
      <el-table-column prop="dept" label="公司名称" />
      <el-table-column prop="ip" label="公司地址" />
      <el-table-column prop="browser" label="电话" />
      <el-table-column prop="loginTime" label="qq" />
      <el-table-column label="操作" width="70px" fixed="right">
        <template slot-scope="scope">
          <el-button slot="reference" size="mini" type="text">详情</el-button>
          <el-button slot="reference" size="mini" type="text">编辑</el-button>
          <el-button slot="reference" size="mini" type="text">删除</el-button>
        </template>
      </el-table-column>
    </el-table>
  </div>
</template>

<script>
// import crudOperation from '@crud/CRUD.operation'
export default {
  name: 'customerList',
  // components: { crudOperation },
  data(){
    return{
       permission: {
        add: ['admin', 'user:add']
      },
    }
  }
}
</script>

<style rel="stylesheet/scss" lang="scss" scoped>
</style>

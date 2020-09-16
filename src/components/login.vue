<template>
    <div class="item">
       <el-form :model="ruleForm" :rules="rules" ref="ruleFormref" label-width="100px">
        <el-form-item label="用户名007" prop="name">
          <el-input v-model="ruleForm.name"></el-input>
        </el-form-item>
        <el-form-item label="密码007" prop="password">
          <el-input v-model="ruleForm.passward"></el-input>
        </el-form-item>
        <el-form-item label="我在改一下看一下？那我提交了再看看" prop="passwords">
          <el-input v-model="ruleForm.passwards"></el-input>
        </el-form-item>
       </el-form>
    </div>

</template>

<script>
export default {
  data () {
    return {
      ruleForm: {
        name: 'admin',
        passward: '123456',
        passwards:''
      }
    }
  }
}
</script>

<style lang="less" scoped>
.item{
    width:500px;
    height: 500px;
    background-color: #eee;
    margin: 0 auto;

}
</style>

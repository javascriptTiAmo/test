<template>
    <div class="item">
       <el-form :model="ruleForm" :rules="rules" ref="ruleFormref" label-width="100px">
        <el-form-item label="刘进进" prop="name">
          <el-input v-model="ruleForm.name"></el-input>
        </el-form-item>
        <el-form-item label="我更改了" prop="password">
          <el-input v-model="ruleForm.passward"></el-input>
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
        passward: '123456'
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

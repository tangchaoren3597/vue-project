<template>
  <div class="container">
    <form>
      <div class="form-group">
        <label>Email address</label>
        <input type="text" class="form-control"  placeholder="请输入姓名" v-model="name">
      </div>
      <div class="form-group">
        <label>Password</label>
        <input type="text" class="form-control" placeholder="请输入地址">
      </div>
      <button class="btn btn-default">提交</button>
    </form>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        name: 'hello world'
      }
    }
  }
</script>

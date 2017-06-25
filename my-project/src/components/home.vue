<template>
  <div class="container top-msg">
    <form class="form-inline">
      <div class="people-msg col-sm-8">
        <div class="form-group">
          <label class="col-sm-3">地址</label>
          <div class="col-sm-5">
            <input type="text" class="form-control"  placeholder="请输入姓名" v-model="name">
          </div>
        </div>
        <button class="btn btn-default">提交</button>
      </div>
    </form>
    <table class="table table-bordered">
      <thead>
          <tr>
            <th>地址</th>
          </tr>
      </thead>
      <tbody>
        <tr v-for=" (people,i) in peoples">
            <td>
              {{people.address}}
            </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        name: 'hello world',
        peoples: [{'address': '杭州'}]
      }
    }
  }
</script>
<style leng="css" scoped>
  /*.top-msg {*/
    /*margin-top: 20px;*/
  /*}*/
  .people-msg {
    margin: 10px auto;
    text-align: center;
  }
</style>

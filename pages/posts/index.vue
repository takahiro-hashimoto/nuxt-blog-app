<template>
  <section class="container">
    <el-card>
      <div slot="header">
        <span>新着投稿</span>
      </div>
      <el-table :data="showPosts" style="width: 100%" class="table">
        <el-table-column prop="title" label="タイトル"></el-table-column>
        <el-table-column prop="user.id" label="投稿者"></el-table-column>
        <el-table-column prop="create_at" label="投稿日"></el-table-column>
      </el-table>
    </el-card>
  </section>
</template>

<script>

export default {
  computed: {
    showPosts() {
      return [
        {
          id: '001',
          title: 'hoge',
          body: 'hogehogehogehogehogehogehogehoge',
          create_at: '2018/12/01 12:00:00',
          user: {
            id: 'takahiro'
          }
        },
        {
          id: '002',
          title: 'fuga',
          body: 'fugafugafugafugafugafugafugafuga',
          create_at: '2018/12/02 12:00:00',
          user: {
            id: 'takahiro'
          }
        },
      ]
    }
  }
}

</script>

<style>

.form-content {
  margin: 16px;
}
</style>

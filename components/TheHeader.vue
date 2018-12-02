<template>
  <el-menu mode="horizontal">
    <el-menu-item index="1" style="pointer-events: none;">
      Nuxt-blog
    </el-menu-item>
    <el-menu-item index="2" style="float: right" :route="{path: '/posts'}">
      投稿一覧
    </el-menu-item>
    <no-ssr>
      <el-menu-item index="4" style="float: right" :route="{path: '/'}">
        <span>ログイン</span>
      </el-menu-item>
    </no-ssr>
    <el-menu-item index="5" style="float: right" :route="{path: '/posts/new'}">
      <span>新規投稿</span>
    </el-menu-item>
  </el-menu>
</template>

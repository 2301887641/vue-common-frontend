<style lang="stylus" scoped>
  .topNav
    .action
      width:97%
      margin:0 auto
      padding:10px 0 10px 5px
      box-sizing:border-box
      background:#fff
      display:flex
      justify-content: space-between
</style>
<template>
  <div class="topNav" style="margin-bottom:15px;">
    <div class="action">
      <span>
        <Button type="error" icon="trash-a" @click="deleteAll">批量删除</Button>
        <Button type="info" icon="ios-search" @click="addView">添加</Button>
      </span>
    </div>
  </div>
</template>

<script>
  export default {
    name: "top-nav",
    data() {
      return {}
    },
    methods: {
      addView() {
        this.$parent.addView()
      },
      deleteAll() {
        this.$parent.deleteAll()
      }
    }
  }
</script>

<template>
  <el-menu
    style="height: 60px"
    class="el-menu-demo"
    mode="horizontal"
    menu-trigger="click"
    size="mini" router>
    <multi-menu v-for="menu of menus" :key="menu.router" :menu="menu"></multi-menu>
  </el-menu>
</template>

<script>
  import MultiMenu from './components/multi-menu.vue'

  export default {
    name: 'KatoMenu',
    components: {
      MultiMenu
    },
    props: {
      /**
       * 菜单数组
       */
      menus: {
        type: Array,
        default: []
      }
    }
  }
</script>

<style lang="less"></style>

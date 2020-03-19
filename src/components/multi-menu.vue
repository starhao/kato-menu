<template>
  <el-submenu
    v-if="menu.children && menu.children.length > 0"
    style="height: 100%;"
    :index="menu.index">
    <template slot="title">
      <i :class="menu.icon"></i>
      <span>{{ menu.label }}</span>
    </template>
    <multi-menu
      v-for="subMenu of menu.children"
      :menu="subMenu"
      :key="subMenu.router">
    </multi-menu>
  </el-submenu>
  <el-menu-item
    v-else
    style="height: 100%;"
    :route="menu.router"
    :index="menu.index">
    <i :class="menu.icon"></i>
    <span>{{ menu.label }}</span>
  </el-menu-item>
</template>

<script>
  export default {
    name: 'multi-menu',
    props: {
      menu: {
        type: Object,
        default: {}
      }
    }
  }
</script>

<style lang="less"></style>

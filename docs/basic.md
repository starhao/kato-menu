基本用法

```vue
<template>
  <kato-menu :menus="menus"/>
</template>

<script>
export default { 

  data() {
    return {
        menus:[
            {index: 'person', router: '/person', label: '随访记录', icon: 'el-icon-notebook-1', 
                children:[
                    {index: 'localDaily', router: '/localDaily', label: '本地筛选日报表'}
                ]
            },
            {index: 'user', router: '/user', label: '录入员管理', icon: 'el-icon-user'},
            {index: 'organization', router: '/organization', label: '组织管理', icon: 'el-icon-house'},
            {index: 'anhuiHealthCheck', router: '/anhuiHealthCheck', label: '来皖摸底排查表'},
        ]   
    }
  }
}
</script>
```
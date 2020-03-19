# kato-menu

[![Build Status](https://badgen.net/travis/starhao/kato-menu/master)](https://travis-ci.com/starhao/kato-menu)
[![NPM Download](https://badgen.net/npm/dm/@starhao/kato-menu)](https://www.npmjs.com/package/@starhao/kato-menu)
[![NPM Version](https://badge.fury.io/js/%40starhao%2Fkato-menu.svg)](https://www.npmjs.com/package/@starhao/kato-menu)
[![NPM License](https://badgen.net/npm/license/@starhao/kato-menu)](https://github.com/starhao/kato-menu/blob/master/LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/starhao/kato-menu/pulls)
[![Automated Release Notes by gren](https://img.shields.io/badge/%F0%9F%A4%96-release%20notes-00B2EE.svg)](https://github-tools.github.io/github-release-notes/)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Install](#install)
- [Usage](#usage)
- [Links](#links)
- [License](#license)

## Introduction

#####基于element-ui的菜单导航栏组件,支持多级别菜单显示.
#####只支持router模式,横向菜单模式

[⬆ Back to Top](#table-of-contents)

## Features

#####支持多层级嵌套菜单

[⬆ Back to Top](#table-of-contents)
## Install
```node
npm install kato-menu
```
[⬆ Back to Top](#table-of-contents)

## Usage
```html
   <kato-menu :menus="menus"/>
```
menus:数组且参数遵循以下格式:
```text
 [
    {index: 'person', router: '/person', label: '随访记录', icon: 'el-icon-notebook-1',
        children:[{index: 'localDaily', router: '/localDaily', label: '本地筛选日报表'}]
    },
    {index: 'user', router: '/user', label: '录入员管理', icon: 'el-icon-user'},
    {index: 'organization', router: '/organization', label: '组织管理', icon: 'el-icon-house'},
    {index: 'anhuiHealthCheck', router: '/anhuiHealthCheck', label: '来皖摸底排查表'},
]   
```

[⬆ Back to Top](#table-of-contents)

## Links

- [docs](https://starhao.github.io/kato-menu/)

[⬆ Back to Top](#table-of-contents)

## License

[MIT](./LICENSE)

[⬆ Back to Top](#table-of-contents)

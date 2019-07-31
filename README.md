# vue-calendar-mobile
仿安卓9.0原生日期选择插件  
基于 CLI3 开发，这可能是全球最小，代码最垃圾的日历插件

### 开发目的

>复刻网易云安卓客户端用，配色也是网易的配色，不喜欢自己改别的色

### 安装

>npm install ka_vue-calendar-mobile --save

### 用法

```html
<calendar :cYear.sync="year" :cMonth.sync="month" :cDate.sync="date" :cDay.sync="day" :cShow.sync="showFlag"></calendar>

<script>
  import calendar from 'ka_vue-calendar-mobile'
  export default {
    data() {
      return {
        showFlag: false,
        year: 1970,
        month: 1,
        date: 1,
        day: 4
      }
    },
    components: { calendar }
  }
</script>

```

### 说明
>所有参数都是同步的修改的，年月日必须传  
:cDay 可以不要，星期用的  
:cShow 可以不要，判断插件是否弹出用

### 为什么不像其他人那样直接输出「年-月-日」

>因为我喜欢
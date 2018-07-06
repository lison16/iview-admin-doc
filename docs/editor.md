# Editor组件

富文本编辑器组件，是对[wangeditor](https://github.com/wangfupeng1988/wangEditor)的简单封装，提供几个属性，你可以根据需要自己拓展。

#### API

- props

属性  |  说明  |  类型  |  默认值
:-------: | -------  |  :-------:  |  :-------:
value | 使用v-model双向绑定，表示当前编辑器内容 | String | ''
valueType | 绑定的值的类型 | enum: ['html', 'text'] | 'html'
changeInterval | 设置change事件触发时间间隔，单位ms | Number | 200
cache | 是否开启本地存储 | Boolean | true

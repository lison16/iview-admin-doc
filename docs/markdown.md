# Markdown组件

富文本编辑器组件，是对[simplemde](https://github.com/sparksuite/simplemde-markdown-editor)的简单封装，提供几个属性，你可以根据需要自己拓展。

#### API

- props

属性  |  说明  |  类型  |  默认值
:-------: | -------  |  :-------:  |  :-------:
value | 使用v-model双向绑定，表示当前编辑器内容 | String | ''
options | simplemde配置项 | Object | {}
localCache | 是否开启本地存储 | Boolean | true

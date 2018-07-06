# Tables组件

Tables组件是对iview表格组件的进一步封装，实现了编辑、删除、按列过滤功能，支持iview所有api，下面仅对拓展功能的api进行介绍。

#### API

- props

属性  |  说明  |  类型  |  默认值
:-------: | -------  |  :-------:  |  :-------:
editable | 全局设置是否可编辑 | Boolean | false
searchable | 是否可搜索 | Boolean | false
searchPlace | 搜索控件所在位置，'top' / 'bottom' | String | 'top'

- events

事件名  |  说明  |  回调函数参数
:-------: | -------  |  :-------:
on-start-edit | 开始编辑时触发 | { row, index, column }
on-cancel-edit | 取消编辑时触发 | { row, index, column }
on-save-edit | 保存编辑时触发 | { row, index, column, value /* 修改后的值 */ }

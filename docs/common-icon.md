# CommonIcon组件

这个组件支持iView内置图标和自定义图标，如果是使用iView内置的图标，则使用方法和使用iView的Icon组件一样；如果是自定义图标，则需要在名字前加上下划线`_`。该组件实际是对iView内置Icon组件和自定义图标组件Icons的结合，而用来区分这两者的就是type属性开头是否带有下划线。

#### API

- props

属性  |  说明  |  类型  |  默认值
:-------: | -------  |  :-------:  |  :-------:
type | 图标名称 | String | -
color | 图标颜色 | String | #5c6b77
size | 图标尺寸 | Number | 16

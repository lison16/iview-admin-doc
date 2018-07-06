# CountTo组件

数字动画效果组件，用来实现数字的动画渐变效果，支持异步更新。

#### API

- props

属性  |  说明  |  类型  |  默认值
:-------: | -------  |  :-------:  |  :-------:
init | 动画未开始时显示的数值 | Number | 0
startVal | 起始值，即动画开始前显示的数值 | Number | 0
end | 结束值，即动画结束后显示的数值 | Number | 必填
decimals | 保留几位小数 | Number | 0
decimal | 分隔整数和小数的符号，默认是小数点 | String | .
duration | 动画持续的时间，单位是秒 | Number | 2
delay | 动画延迟开始的时间，单位是秒 | Number | 0
uneasing | 是否禁用easing动画效果 | Boolean | false
usegroup | 是否使用分组，分组后每三位会用一个符号分隔 | Boolean | false
separator | 用于分组(usegroup)的符号 | String | ,
simplify | 是否简化显示，设为true后会使用unit单位来做相关省略 | Boolean | false
unit | 自定义单位，如[3, 'K+'], [6, 'M+']即大于3位数小于6位数的用k+来做省略1000即显示为1K+ | Array | [[3, 'K+'], [6, 'M+'], [9, 'B+']]
countClass | 应用于数字的自定义类名 | String | -
unitClass | 应用于单位的自定义类名 | String | -

 ## dialog 

::: demo demos/standalone 组件展示
:::

::: demo demos/base 默认
:::

::: demo demos/position 弹框位置
:::

::: demo demos/custom 自定义内容
:::

::: demo demos/others 其他示例
:::

### 属性配置
| 属性 | 类型 | 默认值 | 必传 | 说明 |
|-----|-----|-----|-----|-----|
|visable|Boolean|false|N|用于控制弹框是否显示（v-model）|
|mode|String|'modal'|N|是否模态形式，可选值：'modal', 'not一modal'|
|placement|String|'top'|N|top 定位: 20%，可选值：top/center|
|offset|Object|-|N|offset 是相对于 placement 的偏移量，如offset={left:'100px',top:'200px'}|
|width|String/Number|-|N|对话框宽度，如： 320， '500px'， 80%；如果是数字，单位为px|
|header|Boolean/String/Function|true|N|弹框顶部内容；支持同名插槽（slot）；类型Boolean，表示是否显示；类型String表示为显示内容；类型为Function，则表示渲染函数，函数返回内容将作为渲染结果输出。优先级： Function/String > slot|
|body|Boolean/String/Function|true|N|弹框内容；支持同名插槽（slot）；类型Boolean，表示是否显示；类型String表示为显示内容；类型为Function，则表示渲染函数，函数返回内容将作为渲染结果输出。优先级： Function/String > slot|
|footer|Boolean/String/Function|true|N|弹框底部内容；支持同名插槽（slot）；类型Boolean，表示是否显示；类型String表示为显示内容；类型为Function，则表示渲染函数，函数返回内容将作为渲染结果输出。优先级： Function/String > slot|
|closeBtn|Boolean/Function|true|N|弹框右上角关闭按钮；类型Boolean，表示是否显示关闭按钮；类型为Function ，则表示渲染函数，函数返回内容将作为渲染结果输出。|
|showOverlay|Boolean|true|N|是否显示遮罩层|
|preventScrollThrough|Boolean|true|N|防止滚动穿透|
|draggable|Boolean|'modal'|N|是否允许弹框拖拽，必须要是非模态框（mode='not-modal'）|
|attach|Boolean/String/Function|false|N|指定弹框挂载点，默认子元素挂载；类型Boolean，true挂载document.body，false为子元素挂载；类型String，表示DOM选择器（querySelect）;类型Function，需返回DOM节点，如：()=>document.body|
|zlndex|Number|2500|N|定位层级|
|destroyOnClose|Boolean|false|N|关闭时销毁Dialog子元素|

### 事件event
| 事件名称 | 参数 | 说明 |
|-----|-----|-----|
|keydown-esc|-|按下 ESC 时触发事件|
|click-close-btn|close|关闭按钮点击时触发，组件本身不执行关闭，仅触发事件。执行参数 close 方法，即可关闭弹框。|
|click-overlay|-|点击遮罩层时触发|
|visable-change|visable|弹框状态切换时触发，传递参数visable|
|opened|-|弹框弹出动画结束触发事件，弹出动画暂未实现|
|closed|-|弹框收起动画结束触发事件，收起动画暂未实现|




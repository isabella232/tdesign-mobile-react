:: BASE_DOC ::

## API

### DateTimePicker Props

名称 | 类型 | 默认值 | 说明 | 必传
-- | -- | -- | -- | --
className | String | - | 类名 | N
style | Object | - | 样式，TS 类型：`React.CSSProperties` | N
cancelBtn | String | 取消 | 取消按钮文字 | N
confirmBtn | String | - | 确定按钮文字 | N
end | String / Number | - | 选择器的最大可选时间，默认为当前时间+10年 | N
footer | TElement | true | 底部内容。TS 类型：`TNode`。[通用类型定义](https://github.com/TDesignOteam/tdesign-mobile-react/blob/develop/src/common.ts) | N
format | String | 'YYYY-MM-DD HH:mm:ss' | 用于pick、change、confirm事件参数格式化[详细文档](https://day.js.org/docs/en/display/format) | N
header | TNode | true | 头部内容。值为 true 显示空白头部，值为 false 不显示任何内容，值类型为 TNode 表示自定义头部内容。TS 类型：`boolean | TNode`。[通用类型定义](https://github.com/TDesignOteam/tdesign-mobile-react/blob/develop/src/common.ts) | N
mode | String / Array | 'date' | year = 年；month = 年月；date = 年月日；hour = 年月日时； minute = 年月日时分；当类型为数组时，第一个值控制年月日，第二个值控制时分秒。TS 类型：`DateTimePickerMode` `type DateTimePickerMode = TimeModeValues | Array<TimeModeValues> ` `type TimeModeValues = 'year' | 'month' | 'date' | 'hour' | 'minute' | 'second'`。[详细类型定义](https://github.com/TDesignOteam/tdesign-mobile-react/tree/develop/src/date-time-picker/type.ts) | N
renderLabel | Function | - | 自定义label。TS 类型：`(type: string, value: number) => string` | N
showWeek | Boolean | false | 【开发中】是否在日期旁边显示周几（如周一，周二，周日等） | N
start | String / Number | - | 选择器的最小可选时间，默认为当前时间-10年 | N
title | String | '选择时间' | 标题 | N
value | String / Number | - | 选中值。TS 类型：`DateValue` `type DateValue = string | number`。[详细类型定义](https://github.com/TDesignOteam/tdesign-mobile-react/tree/develop/src/date-time-picker/type.ts) | N
defaultValue | String / Number | - | 选中值。非受控属性。TS 类型：`DateValue` `type DateValue = string | number`。[详细类型定义](https://github.com/TDesignOteam/tdesign-mobile-react/tree/develop/src/date-time-picker/type.ts) | N
visible | Boolean | false | 是否显示 | N
onCancel | Function |  | TS 类型：`(context: { e: MouseEvent }) => void`<br/>取消按钮点击时触发 | N
onChange | Function |  | TS 类型：`(value: DateValue) => void`<br/>value改变时触发 | N
onConfirm | Function |  | TS 类型：`(value: DateValue) => void`<br/>确认按钮点击时触发 | N
onPick | Function |  | TS 类型：`(value: DateValue) => void`<br/>选中值发生变化时触发 | N
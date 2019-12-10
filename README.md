#### cy-element
一些常用的组件，使用react hooks编写
#### install
  npm install cy-element 或者 cnpm install cy-element
#### css3 flex 布局组件
  import { view } from 'cy-element'
#### example
  [组件View布局示例](https://github.com/zyh2123606/cy-element/dist/view.html)
#### property api
property | default | type | values | description
---------| ------- | ---- | ------ | -----------
row      | true    | boolean | true or false | 水平居中
column   | false   | boolean | true or false | 垂直居中
wrap     | false   | boolean | true or false | 换行
flex     | false   | boolean | true or false | 填满剩余空间
around   | false   | boolean | true or false | 平均分布 
justContent | start | string | start, center, end | 水平位置
alignItems  | top   | string | top, middle, bottom | 垂直位置
line        | null  | string | top, left, right, bottom | 0.5像素细线主要用于移动端
###### import { EventEmitter } from 'cy-element'
property | default | type     | description
---------| ------- | ---- | -----------
emit     | void    | Function | 发布事件
listenerEmit | void | Function | 订阅事件
removeListeners | void | Function | 移除订阅的事件
###### EventEmitter.listenerEmit(type, func) 订阅事件
###### EventEmitter.emit(type, args) 发布事件
###### EventEmitter.removeListeners(type, func) 移除事件

#### pc图片预览组件，以横屏或竖屏为基准进行等比缩放，大图预览，支持数组或对象数组['.png']或[{url: '.png'}]，是对象数组的时候可以设置title,显示的标题，不设置则为图片索引加图片数目为图片标题

property | default | type | values | description
---------| ------- | ---- | ------ | -----------
visible  | false   | boolean | true or false | 打开、关闭
data     | empty   | array | array | 图片数组

#### example
  [图片预览示例](https://github.com/zyh2123606/cy-element/dist/picturePreview.html)

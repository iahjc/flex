# flex 布局

## flex容器与flex子项

### flex 容器

flex-direction flex-wrap flex-flow justify-content align-items alingn-content 

### flex 子项

order flex-grow flex-shrink flex-basis flex align-self 

### 改变主轴的方向 flex-direction

flex-direction  : 
        row 默认 横轴方向 从左往右排列
        row-reverse  横轴方向 从右往左排列
        column  竖轴方向 从上往下排列
        column-reverse 竖轴方向 从下往上排列

### 换行与缩写 flex-wrap

    flex-wrap :
        no-wrap 默认
        wrap  折行
        wrap-reverse 反向折行
        column 
        column-reverse

### flex-flow 是 flex-direction flex-wrap的缩写
    flex-flow: cloumn wrap;

### justify-content 主轴对齐
    justify-content:
        flex-start 默认
        flex-end
        center
        space-around
        space-between
        space-evenly

### align-content 交叉轴对齐详解 不折行的情况下 这个属性不生效
    align-content:
        stretch 默认 拉伸 没有高度会自动拉伸
        flex-start
        flex-end 
        center 
        space-around
        space-between
        space-evenly

### align-items  每一行的对其方式
    align-items:
        stretch 
        flex-start
        flex-end
        center
        baseline

## flex子项

order,flex-grow,flex-shrink,flex-basis,flex,align-self

### flex-grow扩展比例
    flex-grow: 0 默认值是0，表示不占用剩余的空白间隙扩展自己的宽度
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
               1 比例指为1，就占满剩余所有的空间
               0.5 比例为0.5 就占有剩余空间的一半
               2 当比例值大于等于1的时候都会占满整个空间

### flex-shrink 收缩比例
    flex-shrink: 默认值是1，表示flex容器空间不足时，元素的收缩比例
                 0.5 溢出部分 收缩一半
                 0 不收缩

### flex-basis及flex缩写
    默认值是auto,指定了flex元素在主轴方向上的初始大小  
    0 最小宽度
    100% 跟容器相同
    固定像素 

### flex 缩写
    flex属性是flex-grow flex-shrink和flex-basis的缩写
    flex：1 表示 flex-grow: 1; flex-shrink: 1; flex-basis: 0%
    flex: 1 表示：flex-grow: 0; flex-shrink:1; flex-basis: 0%
    flex: auto 表示： flex-grow: 1; flex-shrink: 1; flex-basis: auto 
    flex: 1 0 50%

### order 排序
    默认0 改变某一个flex子项的排序位置
    1  优先级低
    -1 优先级低
    
### align-self 
    默认值是auto，控制单独某一个flex子项的垂直对齐方式
    单独控制某一个元素的对其方式
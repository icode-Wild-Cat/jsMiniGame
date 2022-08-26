# 绘制国际象棋棋盘

## canvas元素

==<canvas>==标签在body中建立一个画布，在<script>中写 ==js== 代码以实现画画

```html
<script>
	//创建一个画布对象canv
    const canvas = document.getElementById('canvas')
    //通过getContext(返回canvas的上下文)将画布设定为2D的，对象ctx就相当于我们的画笔了
    const ctx = canvas.getContext("2d")
    //改变画笔颜色
    ctx.fillStyle = 'blue'
    //绘制一个黑色方块
    ctx.fillRect(50,50,100,100)
    //绘制方框(fillStyle颜色不能设定strokeRect颜色,要用strokeRect来设定)
    //fillStyle设定填充颜色
    //strokeStyle设定线条颜色
    ctx.strokeStyle = 'blue'
    //lineWidth设定线条宽度
    ctx.lineWidth = 4
    ctx.strokeRect(50,50,100,100)
</script>
```

JavaScript能够识别上百种颜色的名称，包括**Green、Blue、Orange、Red、Yellow、Purple、White、Black、Pink、Turquoise、Violet、SkyBlue、PaleGreen、Lime、Fuchsia、DeepPink、Cyan、Chocolate**等。

### 绘制线条

**lineTo**：绘制线段


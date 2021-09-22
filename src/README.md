## 1.margin和padding的区别以及应用场景
  1. margin可以为负值；
  2. padding不能为负值；
## 2.关于居中的几种方式讲解
  1. margin:0 auto只能让块级元素进行水平居中并不能让其做到垂直居中
  2. 文字的水平居中text-align:center line-height设为height高度一致
  3. padding填充的方式进行居中，利用padding进行填充然后再用background-clip来进行裁剪
  4. transform:translate(-50%,-50%) -webkit-transform: translate(-50%, -50%);  来进行居中
  5. 绝对定位居中：父级是相对定位position:relative，子元素绝对定位position:absolute 设置top、right、bottom、left为0，并且加上margin:auto记住高度一定是要定义的，并且加上overflow:auto是为了防止内容溢出
  6. 视口居中：利用固定定位 宽度和高度取决于外部容器
  7. 响应式布局
## 3.line-height与vertical-align的理解
  1. line-height行高是指文本行基线之前的距离。行高line-height实际上只影响行内元素和其他行内内容，而不会直接影响块级元素，也可以为一个块级元素设置line-height，但是这个值只是应用到块级元素的内联内容时才会有影响。在应用到块级元素时，line-height定义了元素文本基线之间的最小距离，即最小行高。
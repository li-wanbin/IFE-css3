# IFE-css3 transform

css3中的变形 transform
### 一、变形-旋转 ratate()函数

通过指定的角度参数使元素相对原点进行旋转。它主要在二维空间内进行操作，设置一个角度值，用来指定旋转的幅度。如果这个值为正值，元素相对原点中心顺时针旋转；如果这

个值为负值，元素相对原点中心逆时针旋转。

transform:rotate(-20deg)

 

### 二、变形- 扭曲 skew()函数

扭曲skew()函数能够让元素倾斜显示。它可以将一个对象以其中心位置围绕着X轴和Y轴按照一定的角度倾斜。这与rotate()函数的旋转不同，rotate()函数只是旋转，而不会改变

元素的形状。skew()函数不会旋转，而只会改变元素的形状。

一个参数：表示水平方向的倾斜角度；
两个参数：第一个参数表示水平方向的倾斜角度，第二个参数表示垂直方向的倾斜角度
分3种情况

 transform:skewX(30deg) 



 transform:skewY(10deg) 



 transform:skew(-45deg) 

 

### 三、变形-缩放 scale() 函数

让元素根据中心原点对对象进行缩放。 scale()的取值默认的值为1，当值设置为0.01到0.99之间时，作用使一个元素缩小；而任何大于或等于1.01的值，作用是让元素放大。

也分3种情况：

transform:scale(x,y)  使元素水平方向和垂直方向同时缩放


transform:scale(x)  X轴缩放


 transform:scale(y)  Y轴缩放

 

### 四、变形-位移 translate() 函数

translate()函数可以将元素向指定的方向移动，类似于position中的relative。或以简单的理解为，使用translate()函数，可以把元素从原来的位置移动，而不影响在X、Y轴上

的任何Web组件。

分为三种情况：

transform:translate(x,y)  使元素水平方向和垂直方向同时移动


transform:translate(x)  使元素水平方向移动


transform:translate(y)  使元素垂直方向移动


### 五、变形-原点 transform-origin

 任何一个元素都有一个中心点，默认情况之下，其中心点是居于元素X轴和Y轴的50%处。如下图所示：



在没有重置transform-origin改变元素原点位置的情况下，CSS变形进行的旋转、位移、缩放，扭曲等操作都是以元素自己中心位置进行变形。但很多时候，我们可以通过

transform-origin来对元素进行原点位置改变，使元素原点不在元素的中心位置，以达到需要的原点位置。

transform-origin取值和元素设置背景中的background-position取值类似(也可以是具体的像素值)。





一个在线查看阴影box css值的网站
[https://www.cssmatic.com/box-shadow](https://www.cssmatic.com/box-shadow)

#####手机端📱：
把不是%这种，全部等比例换小，像50px就变成25px，依次替换。
```
        #八卦>div:nth-child(5) {
            /* border: 10px solid rgb(235, 53, 21); */
            width: 50px;
            height: 50px;
            background: black;
            position: absolute;
            left: 50%;
            margin-left: -25px;
            /* 也可以写bottom：0；就下去了 */
            top: 50px;
            border-radius: 50%;
        }

        @media (max-width: 500px) {
            #八卦>div:nth-child(5) {
                width: 25px;
                height: 25px;
                margin-left: -12.5px;
                top: 25px;
            }
        }

```
⚠️ 关键思想：分成了几个div
遮罩用 `overflow: hidden;`

![dao.png](https://upload-images.jianshu.io/upload_images/21001498-2ce54ec83b38e9d0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![dao1.png](https://upload-images.jianshu.io/upload_images/21001498-620caa7ae4693969.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


######动画
两种：
1.animation + @keyframes
2.[animate.css很好简单易用的动画网站](animate.css)
```
animation: x 20s infinite linear;
//把这个x具体化👇
@keyframes x {
    from {
       transform: rotate(0deg)
    }

    to {
        transform: rotate(360deg);
    }
}
```

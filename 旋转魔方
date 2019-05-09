<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Page Title</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" type="text/css" media="screen" href="main.css">
    <script src="main.js"></script>
    <style type="text/css">
        * {
            margin: 0px;
            padding: 0px;
        }

        .container {
            width: 300px;
            height: 300px;
            /* border: 1px solid black;*/
            margin: 150px auto;
            perspective: 20000px;
        }

        .box {
            width: 300px;
            height: 300px;
            transform-style: preserve-3d;
            /*transform: rotateX(45deg) rotateY(45deg);*/
            animation: ro 4s linear infinite;
        }

        @keyframes ro {
            0% {
                transform: rotateX(0deg) rotateY(0deg)
            }

            100% {
                transform: rotateX(360deg) rotateY(360deg)
            }
        }

        .box-page {
            width: 300px;
            height: 300px;
            position: absolute;
            transform-style: preserve-3d;
        }

        .top {
           /* background-color: red;*/
            transform: translateZ(150px);
        }

        .bottom {
           /* background-color: green;*/
            transform: translateZ(-150px) rotateX(180deg);
            /*少了180*/
        }

        .left {
           /* background-color: orange;*/
            transform: translateX(-150px) rotateY(-90deg);
        }

        /*正90*/

        .right {
            /*background-color: pink;*/
            transform: translateX(150px) rotateY(90deg);
        }

        .before {
            /*background-color: blue;*/
            transform: translateY(150px) rotateX(-90deg);
            /*正90*/
        }

        .after {
            /*background-color: yellow;*/
            transform: translateY(-150px) rotateX(90deg);
        }

        .box-page div:nth-child(1) {
            animation: A1 4.5s ease-in;
        }
        .box-page div:nth-child(2) {
            animation: A1 4.5s ease-in 0.5s;
        }
        .box-page div:nth-child(3) {
            animation: A1 4.5s ease-in 1.0s;
        }
        .box-page div:nth-child(4) {
            animation: A1 4.5s ease-in 1.5s;
        }
        .box-page div:nth-child(5) {
            animation: A1 4.5s ease-in 2.0s;
        } .box-page div:nth-child(6) {
            animation: A1 4.5s ease-in 2.5s;
        }
        .box-page div:nth-child(7) {
            animation: A1 4.5s ease-in 3.0s;
        }
        .box-page div:nth-child(8) {
            animation: A1 4.5s ease-in 3.5s;
        }
        .box-page div:nth-child(9) {
            animation: A1 4.5s ease-in 4.0s;
        }
        @keyframes A1 {
            0% {
                transform: translateZ(0px) scale(1) rotateZ(0deg)
            }

           20% {
                transform: translateZ(300px) scale(0) rotateZ(720deg)
            }

            90% {
                transform: translateZ(300px) scale(0) rotateZ(720deg)
            }

            100% {
                transform: translateZ(0px) scale(1) rotateZ(0deg)
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="box">
            <div class="box-page top"></div>
            <div class="box-page bottom"></div>
            <div class="box-page left"></div>
            <div class="box-page right"></div>
            <div class="box-page before"></div>
            <div class="box-page after"></div>
        </div>
    </div>
    <script type="text/javascript">
        var arr = document.querySelectorAll(".box-page");
        for (var n = 0; n < arr.length; n++) { //面
            for (var r = 0; r < 3; r++) { //行
                for (var l = 0; l < 3; l++) { //列
                    var divs = document.createElement("div");
                    divs.style.cssText =
                        "width:100px;height:100px;border:2px solid #fff;box-sizing:border-box;background-image:url(img/A" +
                        n + ".jpg);position:absolute;background-size:300px 300px";
                    arr[n].appendChild(divs);
                    divs.style.left = l * 100 + "px";
                    divs.style.top = r * 100 + "px";
                    divs.style.backgroundPositionX = -l * 100 + "px";
                    divs.style.backgroundPositionY = -r * 100 + "px";
                }
            }
        }
    </script>
</body>

</html>

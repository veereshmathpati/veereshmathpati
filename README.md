<html>
<head>
    <title>canavas</title>
    <style>
        canvas{
            border:solid 1px red;
            margin: 10px;
        }
    </style>
</head>
<body>
    <p>default canvas</p>
    <canvas></canvas>
    <P>rect canvas</P>
    <canvas id="rect" width="200" height="200"></canvas>
    <script>
        a=document.getElementById("rect");
        b=a.getContext("2d");
        b.fillStyle="red";
        b.fillRect(50,50,100,100);
        b.globalAlpha=0.50;

        b=a.getContext("2d");
        b.fillStyle="green";
        b.fillRect(75,75,100,100);
        b.globalAlpha=0.50;
    </script>
    <canvas id="circle" width="200" height="200"></canvas>
    <script>
        a=document.getElementById("circle");
        b=a.getContext("2d");
        b.beginPath();
        b.fillStyle="red";
        b.arc(100,100,30,0,2*3.142);
        b.fill();

        b=a.getContext("2d");
        b.beginPath();
        b.fillStyle="green";
        b.arc(75,75,30,0,2*3.142);
        b.fill();

        b=a.getContext("2d");
        b.beginPath();
        b.fillStyle="blue";
        b.arc(125,125,30,0,2*3.142);
        b.fill();
    </script>
     <canvas id="line" width="200" height="200"></canvas>
     <script>
        a=document.getElementById("line");
        b=a.getContext("2d");
        b.moveTo(0,0);
        b.lineTo(200,200);
        b.stroke();
     </script>
</body>
</html>

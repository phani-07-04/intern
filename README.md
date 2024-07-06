<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ALBUM</title>
</head>
<body>
    <div class="full" id="fullImgBox">
        <img src="./ca.goku1.webp" id="fullImg">
        <span onclick="closeFullImg()">x</span>
    </div>
    <link rel="stylesheet" href="dbz.css">

    <h1 style="color: white;display:flex;justify-content: center;align-items: center;padding-top: 30px;font-family: cursive;font-size: 50px;">DRAGON BALL Z ALBUM</h1>

     <h2>
    <div class="container">
       
        <div class="images">
            <img src="./ca.goku1.webp" onclick="openImage(this,src)">
            <img src="./ca.vegeta.webp" onclick="openImage(this.src)">
            <img src="./trunks.webp" onclick="openImage(this.src)">
            <img src="./ca.gohan.webp" onclick="openImage(this.src)">
            <img src="./broly.webp" onclick="openImage(this.src)">
            <img src="./ca.lord beerus.webp" onclick="openImage(this.src)">
            <img src="jiren.webp" onclick="openImage(this.src)">
            <img src="./ca.zeno.webp" onclick="openImage(this.src)">
        </div>
    </div>
    </h2>
    <script>
          var fullImgBox = document.getElementById("fullImgBox");
          var fullImg = document.getElementById("fullImg");
          function openImage(pic){
            fullImgBox.style.display = "flex";
            fullImg.src = pic;
          }
          function closeFullImg(){
            fullImgBox.style.display = "none";
          }
    </script>
</body>
</html>

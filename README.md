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

*/css file 

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body{
    background-color: rgba(8, 8, 9, 0.3);
}
.container{
    width: 100%;
    height: 100vh;
    margin-left: 10px;
    margin-top: 10;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: none;

}
.images img{
    height: 300px;
    width: 450px;
    padding: 20px;
    cursor: pointer;
    opacity: none;
  }
  .images img:hover{
    transform: scale(0.8) rotate(-15deg);
    border-radius: 10px;
    box-shadow: 0 32px 75px rgba(68, 72, 136, 0.2);
  }
  .full {
    background-color: rgba(0, 0, 0,0.9);
    left : 0;
    top : 0;
    width: 100%;
    height:100vh;
    position: fixed;
    display: none;
    justify-content: center;
    align-items: center;
  }
  .full img{
    width: 90%;
    max-width: 700px;
  }
  .full span{
position: absolute;
top: 25%;
right: 25%;
font-size: 30px;
color: white;
cursor: pointer;
  }

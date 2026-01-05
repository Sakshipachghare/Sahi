<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>I love you Sahi</title>
<style>
body{
  margin:0;
  font-family: Arial, sans-serif;
  background:#000;
  color:#fff;
  overflow:hidden;
}
.slider{
  position:relative;
  width:100vw;
  height:100vh;
}
.slide{
  position:absolute;
  width:100%;
  height:100%;
  background-size:cover;
  background-position:center;
  opacity:0;
  animation:fade 20s infinite;
}
.slide:nth-child(1){animation-delay:0s;}
.slide:nth-child(2){animation-delay:5s;}
.slide:nth-child(3){animation-delay:10s;}
.slide:nth-child(4){animation-delay:15s;}

@keyframes fade{
  0%{opacity:0;}
  10%{opacity:1;}
  25%{opacity:1;}
  35%{opacity:0;}
  100%{opacity:0;}
}

/* Moving caption */
.caption{
  position:absolute;
  font-size:22px;
  font-weight:bold;
  color:#fff;
  animation:move 8s infinite alternate;
}

@keyframes move{
  0%{top:10%; left:10%;}
  25%{top:70%; left:20%;}
  50%{top:40%; left:60%;}
  75%{top:20%; left:70%;}
  100%{top:60%; left:10%;}
}

.music{
  position:fixed;
  bottom:20px;
  left:50%;
  transform:translateX(-50%);
}
button{
  padding:10px 16px;
  border:none;
  border-radius:20px;
  background:#fff;
  color:#000;
  font-weight:bold;
}
</style>
</head>
<body>

<div class="slider">
  <!-- Replace image names with your photos -->
  <div class="slide" style="background-image:url('photo1.jpg')"></div>
  <div class="slide" style="background-image:url('photo2.jpg')"></div>
  <div class="slide" style="background-image:url('photo3.jpg')"></div>
  <div class="slide" style="background-image:url('photo4.jpg')"></div>

  <div class="caption">I love you Sahi…💗😚</div>
</div>

<div class="music">
  <audio id="song" src="saiyaara.mp3"></audio>
  <button onclick="document.getElementById('song').play()">▶ Play Music</button>
</div>

</body>
</html>

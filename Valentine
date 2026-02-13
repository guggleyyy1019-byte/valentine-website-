<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Manish ❤️</title>
<style>
body{
  margin:0;
  font-family:Georgia,serif;
  background:radial-gradient(circle at top,#1a001a,#000);
  color:white;
  text-align:center;
  overflow:hidden;
}
.container{
  max-width:650px;
  margin:0 auto;
  padding:40px 20px;
  position:relative;
  z-index:2;
}
h1{font-size:34px;}
p{font-size:18px;line-height:1.6;}
button{
  padding:14px 28px;
  font-size:16px;
  margin:15px;
  border-radius:30px;
  border:none;
  cursor:pointer;
}
#yes{background:#ff4d88;color:white;box-shadow:0 0 20px #ff4d88;transition:0.3s;}
#no{background:#555;color:white;transition:0.3s;}
#no:hover{transform:scale(1.2);}
.heart{
  position:fixed;
  bottom:-20px;
  font-size:20px;
  animation:float 7s linear infinite;
}
@keyframes float{
0%{transform:translateY(0);}
100%{transform:translateY(-110vh);}
}
.slideshow{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  z-index:1;
  opacity:0.15;
}
.slideshow img{
  position:absolute;
  width:100%;
  height:100%;
  object-fit:cover;
  animation:fade 15s infinite;
}
.slideshow img:nth-child(2){animation-delay:5s;}
.slideshow img:nth-child(3){animation-delay:10s;}
@keyframes fade{
0%{opacity:0;}
10%{opacity:1;}
30%{opacity:1;}
40%{opacity:0;}
100%{opacity:0;}
}
</style>
</head>
<body>

<!-- Photo Slideshow -->
<div class="slideshow">
  <img src="photo1.jpg">
  <img src="photo2.jpg">
  <img src="photo3.jpg">
</div>

<div class="container" id="content">
<h1>Four years… and it’s still you.</h1>
<p>Through every version of us — I’d still choose you.</p>
<button onclick="nextPage(1)">Next</button>
</div>

<script>
const pages=[
{title:"We’ve grown.",text:"Not perfectly. Not always easily. But together."},
{title:"And if I had to start over?",text:"I’d still find you. In every lifetime. Until I found you… and I’d find you again."},
{title:"So Manish…",text:"<strong style='font-size:28px;'>Will you be my Valentine? 💖</strong><br><br><button id='yes' onclick='yesClicked()'>YES ❤️</button><button id='no' onmouseover='moveNo()'>No 😢</button>"}];

function nextPage(index){
document.getElementById("content").innerHTML=
"<h1>"+pages[index].title+"</h1><p>"+pages[index].text+"</p>"+
(index<pages.length-1?"<button onclick='nextPage("+(index+1)+")'>Next</button>":"");
}

function yesClicked(){
document.body.innerHTML="<div style='text-align:center;margin-top:20%;'><h1 style='font-size:50px;'>YAY ❤️</h1><p style='font-size:22px;'>Still choosing you. Always.</p><div id='confetti' style='font-size:40px;'>💖 💕 💗 💘 💞</div></div>";
for(let i=0;i<70;i++){createHeart();}
}

function moveNo(){
const btn=document.getElementById('no');
btn.style.position='absolute';
btn.style.left=Math.random()*80+'%';
btn.style.top=Math.random()*80+'%';
}

function createHeart(){
const heart=document.createElement('div');
heart.className='heart';
heart.innerHTML='💖';
heart.style.left=Math.random()*100+'vw';
document.body.appendChild(heart);
setTimeout(()=>heart.remove(),7000);
}
setInterval(createHeart,400);

/* Surprise message after 5 seconds */
setTimeout(()=>{alert("You make my world softer. 💕");},5000);
</script>
</body>
</html>

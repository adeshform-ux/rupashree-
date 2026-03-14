<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Rupashree 🎂</title>

<style>

body{
margin:0;
font-family:Arial;
background:linear-gradient(135deg,#ff9a9e,#fad0c4);
display:flex;
justify-content:center;
align-items:center;
height:100vh;
overflow:hidden;
text-align:center;
}

.container{
background:white;
padding:40px;
border-radius:20px;
box-shadow:0 10px 30px rgba(0,0,0,0.2);
max-width:420px;
}

h1{
color:#ff4d6d;
}

button{
padding:12px 25px;
font-size:18px;
border:none;
border-radius:25px;
background:#ff4d6d;
color:white;
cursor:pointer;
margin-top:20px;
}

.hidden{
display:none;
}

.cake{
font-size:80px;
animation:bounce 2s infinite;
}

@keyframes bounce{
0%,100%{transform:translateY(0)}
50%{transform:translateY(-10px)}
}

.balloon{
position:absolute;
font-size:30px;
animation:floatUp 10s linear infinite;
}

@keyframes floatUp{
0%{transform:translateY(100vh);}
100%{transform:translateY(-10vh);}
}

.heart{
position:absolute;
font-size:20px;
color:red;
animation:floatUp 6s linear infinite;
}

.confetti{
position:absolute;
width:10px;
height:10px;
animation:fall 3s linear infinite;
}

@keyframes fall{
0%{transform:translateY(-10vh);}
100%{transform:translateY(100vh);}
}

#message{
font-size:18px;
margin-top:10px;
min-height:60px;
}

</style>
</head>

<body>

<audio id="music" loop>
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
</audio>

<div class="container" id="gift">

<h1>🎁 A Special Gift</h1>
<p>Click to open your birthday surprise</p>

<button onclick="openGift()">Open Gift 🎉</button>

</div>


<div class="container hidden" id="birthday">

<h1>🎂 Happy Birthday Rupashree ❤️</h1>

<div class="cake">🎂</div>

<p id="message"></p>

</div>


<script>

function openGift(){

document.getElementById("gift").style.display="none";
document.getElementById("birthday").style.display="block";

document.getElementById("music").play();

startHearts();
startConfetti();
startBalloons();
typeMessage();

}

function startHearts(){
setInterval(()=>{
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
document.body.appendChild(heart);

setTimeout(()=>heart.remove(),6000);

},400);
}

function startConfetti(){
setInterval(()=>{
let confetti=document.createElement("div");
confetti.className="confetti";
confetti.style.left=Math.random()*100+"vw";
confetti.style.background=["red","blue","yellow","green","pink"][Math.floor(Math.random()*5)];
document.body.appendChild(confetti);

setTimeout(()=>confetti.remove(),3000);

},200);
}

function startBalloons(){
setInterval(()=>{
let balloon=document.createElement("div");
balloon.className="balloon";
balloon.innerHTML="🎈";
balloon.style.left=Math.random()*100+"vw";
document.body.appendChild(balloon);

setTimeout(()=>balloon.remove(),10000);

},1500);
}

function typeMessage(){

let text="Wishing you a day filled with love, happiness and beautiful moments. You are very special Rupashree ❤️";
let i=0;

let speed=60;

function typing(){
if(i<text.length){
document.getElementById("message").innerHTML+=text.charAt(i);
i++;
setTimeout(typing,speed);
}
}

typing();

}

</script>

</body>
</html>

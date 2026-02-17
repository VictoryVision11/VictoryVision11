
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Victory Vision | Premium Cricket Insights</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:linear-gradient(135deg,#050816,#0d132b);
color:white;
text-align:center;
overflow-x:hidden;
}

/* PROFILE */
.profile{
padding:40px 20px;
}

.profile img{
width:110px;
height:110px;
border-radius:50%;
border:3px solid #00f0ff;
box-shadow:0 0 25px #00f0ff;
}

.profile h1{
margin-top:15px;
font-size:24px;
font-weight:700;
}

.followers{
color:#00f0ff;
font-size:14px;
margin-top:5px;
}

/* STATS */
.stats{
display:flex;
justify-content:center;
gap:15px;
flex-wrap:wrap;
margin-top:25px;
}

.stat-box{
background:rgba(255,255,255,0.05);
backdrop-filter:blur(10px);
padding:15px;
border-radius:15px;
width:110px;
box-shadow:0 0 20px rgba(0,255,255,0.3);
transition:0.3s;
}

.stat-box:hover{
transform:scale(1.05);
}

.stat-box h2{
font-size:20px;
color:#00f0ff;
}

.stat-box span{
font-size:11px;
opacity:0.8;
}

/* TELEGRAM BUTTON */
.telegram-btn{
display:inline-block;
margin:35px auto;
padding:15px;
width:85%;
border-radius:40px;
background:linear-gradient(90deg,#00c6ff,#a100ff);
color:white;
font-weight:600;
text-decoration:none;
box-shadow:0 0 25px rgba(161,0,255,0.8);
transition:0.3s;
}

.telegram-btn:hover{
transform:scale(1.05);
}

/* COUNTDOWN */
.countdown{
margin:20px;
padding:20px;
border-radius:20px;
background:rgba(255,255,255,0.05);
backdrop-filter:blur(15px);
box-shadow:0 0 25px rgba(0,255,255,0.3);
}

.countdown h3{
color:#00f0ff;
margin-bottom:15px;
}

.time{
display:flex;
justify-content:space-around;
font-size:18px;
}

.time div span{
display:block;
font-size:10px;
opacity:0.7;
}

/* FEATURES */
.feature{
margin:20px;
padding:20px;
border-radius:20px;
background:rgba(255,255,255,0.05);
backdrop-filter:blur(15px);
box-shadow:0 0 20px rgba(161,0,255,0.4);
text-align:left;
transition:0.3s;
}

.feature:hover{
transform:translateY(-5px);
}

.feature h4{
margin-bottom:8px;
color:#a100ff;
font-size:16px;
}

.feature p{
font-size:13px;
opacity:0.8;
}

footer{
margin:30px 0;
font-size:12px;
opacity:0.5;
}
</style>
</head>

<body>

<section class="profile">
<img src=https://ibb.co/BV3n4gqalt="Profile">
<h1>Victory Vision</h1>
<p class="followers">29.8K Followers</p>
</section>

<section class="stats">
<div class="stat-box">
<h2 id="subs">0</h2>
<span>Subscribers</span>
</div>

<div class="stat-box">
<h2 id="pred">0</h2>
<span>Predictions</span>
</div>

<div class="stat-box">
<h2>96%</h2>
<span>Accuracy</span>
</div>
</section>

<a href=https://t.me/+ZCNMoT7JzUIzNDU1_blank" class="telegram-btn">
🚀 Join Telegram Channel
</a>

<section class="countdown">
<h3>Next Prediction In</h3>
<div class="time">
<div id="days">00<span>Days</span></div>
<div id="hours">00<span>Hours</span></div>
<div id="minutes">00<span>Minutes</span></div>
<div id="seconds">00<span>Seconds</span></div>
</div>
</section>

<div class="feature">
<h4>⏰ Pre-match Analysis</h4>
<p>Expert match breakdown before every game with high accuracy insights.</p>
</div>

<div class="feature">
<h4>✔ Transparent Results</h4>
<p>Complete performance history with verified records.</p>
</div>

<div class="feature">
<h4>🔔 Live Alerts</h4>
<p>Instant updates and smart insights during live matches.</p>
</div>

<footer>
© 2026 Victory Vision | All Rights Reserved
</footer>

<script>
/* Animated Counter */
function animateValue(id, start, end, duration) {
let range = end - start;
let current = start;
let increment = end > start ? 1 : -1;
let stepTime = Math.abs(Math.floor(duration / range));
let obj = document.getElementById(id);
let timer = setInterval(function() {
current += increment;
obj.textContent = current.toLocaleString();
if (current == end) clearInterval(timer);
}, stepTime);
}

animateValue("subs", 0, 29856, 2000);
animateValue("pred", 0, 1547, 2000);

/* Countdown Timer (24 Hour Example) */
let countDownDate = new Date().getTime() + (24 * 60 * 60 * 1000);

setInterval(function() {
let now = new Date().getTime();
let distance = countDownDate - now;

let days = Math.floor(distance / (1000 * 60 * 60 * 24));
let hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
let minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
let seconds = Math.floor((distance % (1000 * 60)) / 1000);

document.getElementById("days").innerHTML = days + "<span>Days</span>";
document.getElementById("hours").innerHTML = hours + "<span>Hours</span>";
document.getElementById("minutes").innerHTML = minutes + "<span>Minutes</span>";
document.getElementById("seconds").innerHTML = seconds + "<span>Seconds</span>";

}, 1000);
</script>

</body>
</html>

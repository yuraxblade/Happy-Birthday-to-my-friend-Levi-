<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Levi 🎉</title>

<style>
body{
  margin:0;
  height:100vh;
  background:linear-gradient(135deg,#fbc2eb,#a6c1ee);
  display:flex;
  justify-content:center;
  align-items:center;
  font-family: Arial, sans-serif;
  overflow:hidden;
}

.card{
  background:#fff;
  padding:30px;
  border-radius:18px;
  text-align:center;
  width:90%;
  max-width:420px;
  box-shadow:0 15px 35px rgba(0,0,0,0.2);
  animation:fadeIn 1.2s ease;
}

h1{
  color:#5a4fcf;
  margin-bottom:15px;
}

p{
  color:#444;
  font-size:16px;
  line-height:1.6;
}

.float{
  position:fixed;
  bottom:-40px;
  font-size:26px;
  animation:up 6s linear infinite;
  opacity:0.9;
}

@keyframes up{
  0%{transform:translateY(0) scale(1);opacity:1;}
  100%{transform:translateY(-110vh) scale(1.4);opacity:0;}
}

@keyframes fadeIn{
  from{opacity:0; transform:scale(0.8);}
  to{opacity:1; transform:scale(1);}
}
</style>
</head>

<body>

<div class="card">
  <h1>🎂 Happy Birthday Levi 🎂</h1>

  <p>
    Hey Levi 🤗<br><br>
    Today is your special day and I just wanted to remind you
    how appreciated you are.<br><br>
    May this year bring you calm moments, genuine smiles,
    and everything that makes you feel happy inside.<br><br>
    Sending you warm hugs and good vibes 🌹💙
  </p>

  <p><i>— Your friend</i></p>
</div>

<script>
const items = ["🌹","❤️","🤗","💐"];

function floatItem(){
  const el = document.createElement("div");
  el.className = "float";
  el.innerText = items[Math.floor(Math.random()*items.length)];
  el.style.left = Math.random()*100 + "vw";
  el.style.animationDuration = (4 + Math.random()*3) + "s";
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),7000);
}

setInterval(floatItem,500);
</script>

</body>
</html>

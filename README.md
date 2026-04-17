<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dilshodbek | Developer</title>
<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
  color: white;
}

header {
  text-align: center;
  padding: 60px 20px;
}

h1 {
  font-size: 3em;
}

.typewriter {
  overflow: hidden;
  border-right: .15em solid white;
  white-space: nowrap;
  animation: typing 4s steps(40, end), blink .75s step-end infinite;
}

@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

@keyframes blink {
  from, to { border-color: transparent }
  50% { border-color: white }
}

.card {
  background: rgba(255,255,255,0.05);
  margin: 20px auto;
  padding: 20px;
  border-radius: 20px;
  width: 80%;
  backdrop-filter: blur(10px);
}

button {
  padding: 10px 20px;
  border: none;
  border-radius: 10px;
  background: #00c6ff;
  color: black;
  cursor: pointer;
}

.progress {
  background: #333;
  border-radius: 10px;
  overflow: hidden;
  margin: 10px 0;
}

.progress-bar {
  height: 10px;
  background: #00ffcc;
}

footer {
  text-align: center;
  padding: 20px;
  opacity: 0.7;
}
</style>
</head>
<body>

<header>
  <h1>Dilshodbek Sattarov</h1>
  <p class="typewriter">Frontend Developer | Telegram Bot Lover | IT Student</p>
</header>

<div class="card">
  <h2>Men haqimda</h2>
  <p>Men dasturlashga qiziqaman. Ayniqsa HTML, CSS, JavaScript va Telegram botlar yaratish yoqadi.</p>
</div>

<div class="card">
  <h2>Ko'nikmalar</h2>
  <p>HTML</p>
  <div class="progress"><div class="progress-bar" style="width: 90%"></div></div>
  <p>CSS</p>
  <div class="progress"><div class="progress-bar" style="width: 85%"></div></div>
  <p>JavaScript</p>
  <div class="progress"><div class="progress-bar" style="width: 70%"></div></div>
</div>

<div class="card">
  <h2>Statistika</h2>
  <p>Saytga kiruvchilar soni:</p>
  <h1 id="counter">0</h1>
  <!-- BU YERGA API yoki backend orqali real statistika qo'shish mumkin -->
</div>

<div class="card">
  <h2>Telegram Botlar</h2>
  <p>Men Telegram botlar yaratishga qiziqaman va API bilan ishlashni o'rganmoqdaman.</p>
  <button onclick="showAlert()">Meni bos!</button>
</div>

<footer>
  <p>© 2026 Dilshodbek | GitHub Profile</p>
</footer>

<script>
let count = localStorage.getItem('visits') || 0;
count++;
localStorage.setItem('visits', count);
document.getElementById('counter').innerText = count;

function showAlert() {
  alert("Salom! Sen mening GitHub profilimni ko'ryapsan 😎");
}
</script>

</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Happy New Year Bangaram</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #fffaf5;
  text-align: center;
}

.screen {
  display: none;
  min-height: 100vh;
  padding: 30px;
  box-sizing: border-box;
}

.active {
  display: block;
}

button {
  padding: 14px 26px;
  border: none;
  background: #d32f2f;
  color: white;
  font-size: 16px;
  border-radius: 30px;
  cursor: pointer;
  margin-top: 20px;
}

h1 {
  color: #8b0000;
}

img {
  max-width: 200px;
  border-radius: 20px;
}
</style>
</head>

<body>

<!-- SCREEN 1 -->
<div class="screen active" id="screen1">
  <img src="https://images.unsplash.com/photo-1514888286974-6c03e2ca1dba?w=300">
  <h1>Happy New Year 🎉</h1>
  <h2>Bangaram 😘</h2>
  <p>Thanks for being part of my 2025 💖</p>
  <button onclick="next(1)">Continue →</button>
</div>

<!-- SCREEN 2 -->
<div class="screen" id="screen2">
  <h1>Goals for 2026 ✨</h1>
  <p>🌍 Travel more</p>
  <p>📚 Learn new things</p>
  <p>❤️ Take care of yourself</p>
  <button onclick="next(2)">Next →</button>
</div>

<!-- SCREEN 3 -->
<div class="screen" id="screen3">
  <h1>A Small Message 💌</h1>
  <p>You matter more than you know.</p>
  <p>Never forget that 🤍</p>
  <button onclick="next(3)">Open Surprise 🎁</button>
</div>

<!-- SCREEN 4 -->
<div class="screen" id="screen4">
  <h1>🎆 Happy New Year 2026 🎆</h1>
  <p>May this year be kind, bright and full of love 💫</p>
  <h2>— For You, Bangaram 💛</h2>
  <button onclick="location.reload()">Restart 🔁</button>
</div>

<script>
function next(n) {
  document.getElementById("screen" + n).classList.remove("active");
  document.getElementById("screen" + (n+1)).classList.add("active");
}
</script>

</body>
</html>

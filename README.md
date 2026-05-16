# uzmi index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Uzmi ❤️</title>

<style>
body {
  margin: 0;
  padding: 0;
  background: black;
  font-family: Arial, sans-serif;
  text-align: center;
  color: white;
  overflow: hidden;
}

h1 {
  margin-top: 80px;
  font-size: 35px;
  background: linear-gradient(to right, pink, violet);
  -webkit-background-clip: text;
  color: transparent;
  animation: fadeIn 2s ease-in-out;
}

p {
  font-size: 18px;
  opacity: 0;
  transition: 1s;
}

button {
  margin-top: 30px;
  padding: 12px 25px;
  border: none;
  border-radius: 25px;
  background: linear-gradient(to right, pink, violet);
  color: white;
  font-size: 16px;
  cursor: pointer;
}

.cake {
  font-size: 70px;
  margin-top: 20px;
  animation: bounce 2s infinite;
}

@keyframes fadeIn {
  from {opacity: 0; transform: scale(0.5);}
  to {opacity: 1; transform: scale(1);}
}

@keyframes bounce {
  0%,100% {transform: translateY(0);}
  50% {transform: translateY(-15px);}
}

.heart {
  position: absolute;
  color: pink;
  font-size: 20px;
  animation: float 5s linear infinite;
}

@keyframes float {
  from {transform: translateY(100vh);}
  to {transform: translateY(-10vh);}
}
</style>

</head>

<body>

<h1>Happy Birthday Uzmi ❤️</h1>

<div class="cake">🎂</div>

<button onclick="showMessage()">Click for Surprise 🎁</button>

<p id="msg">
Happy Birthday Uzmi 💖 <br>
You are the most special person in my life 😘 <br>
I love you so much ❤️ <br>
Stay happy forever 🎉
</p>

<script>
function showMessage() {
  document.getElementById("msg").style.opacity = "1";
}

setInterval(() => {
  let heart = document.createElement("div");
  heart.innerHTML = "❤️";
  heart.className = "heart";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.fontSize = Math.random() * 20 + 10 + "px";
  document.body.appendChild(heart);

  setTimeout(() => {
    heart.remove();
  }, 5000);
}, 300);
</script>

</body>
</html>

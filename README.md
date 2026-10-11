<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title> Sorry o deha maaf kor daa please ❤️</title><style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ffb6c1, #ff69b4, #ffc0cb);
    color: #8b003a;
    text-align: center;
    overflow-x: hidden;
    padding: 20px;
}

.card {
    background: rgba(255,255,255,0.94);
    padding: 30px 22px;
    border-radius: 25px;
    max-width: 430px;
    width: 100%;
    box-shadow: 0 10px 35px rgba(150,0,60,0.2);
    position: relative;
    z-index: 1;
}

.heart {
    font-size: 65px;
    animation: beat 1s infinite;
}

h1 {
    color: #ff1493;
}

p {
    line-height: 1.8;
}

button {
    border: none;
    border-radius: 30px;
    padding: 14px 22px;
    margin: 8px;
    font-size: 16px;
    cursor: pointer;
}

#yes {
    background: #ff1493;
    color: white;
}

#message {
    display: none;
    margin-top: 20px;
    font-size: 19px;
    font-weight: bold;
}

.floating {
    position: fixed;
    bottom: -30px;
    animation: float 7s linear infinite;
    pointer-events: none;
}

@keyframes beat {
    50% { transform: scale(1.2); }
}

@keyframes float {
    to {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
    }
}
</style></head><body><div class="card">
    <div class="heart">❤️</div><h1>I'm Sorry, My Love 🥺</h1>

<h3>To My Special Person 💗</h3>

<p>
    O sumu maaf kori diya na please hoi jai aru vul.
  moi khong te koi dilu oo jiti, online thakiu message seen 
  kora nai jeen. henekwa nokoriba na please..Love you oo deha.
<p>
    Hoi baru moi jee khini kolu hai2 bodlabo nwaru.
  Moi je khini kolu khong t he kolu monor pora ekua kwa nai oo.
  Moi jiti khn koi dew aru khong t khali kamakhya hopot etaw kotha monor 
  pora kwa nai .🥹
</p>

<h3> Maaf kori diya naa aiii piliz....pilizz 💌</h3>

<button id="yes" onclick="forgive()">
    Maaf kori dilu Bidu mainak❤️
</button>

<button onclick="showLove()">
    Read My Promise 💖
</button>

<div id="message"></div>

</div><script>
function forgive() {
    document.getElementById("message").style.display = "block";
    document.getElementById("message").innerHTML =
        "Thank you, Oo deha! ❤️🥹 Tumi nohole thakibo nwaru oo deha! uu maaah love uuuuuu....! 🫂💗";
    burstHearts();
}

function showLove() {
    document.getElementById("message").style.display = "block";
    document.getElementById("message").innerHTML =
        "Moi hosake koisu ajir pora henke ekua nokow ekodm kamakhya hopot, mur mane kwa paost nijore mon tu baya lagi ase kio nu kolu. ❤️🌹";
}

function burstHearts() {
    for (let i = 0; i < 25; i++) {
        const heart = document.createElement("div");
        heart.textContent = ["❤️", "💗", "💕", "💖"][Math.floor(Math.random() * 4)];
        heart.className = "floating";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = (3 + Math.random() * 4) + "s";
        heart.style.fontSize = (18 + Math.random() * 20) + "px";
        document.body.appendChild(heart);
        setTimeout(() => heart.remove(), 7000);
    }
}
</script></body>
</html>

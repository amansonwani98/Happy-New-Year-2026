<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year 2026 - Mela Pyala Bacchaaa ❤️</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
/* Body & background */
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #222;
    overflow-x: hidden;
    color: #fff;
    text-align: center;
}

/* Confetti animation */
.confetti {
    position: fixed;
    width: 10px;
    height: 10px;
    background-color: #ff2f92;
    top: -10px;
    animation: fall linear infinite;
    border-radius: 50%;
    opacity: 0.8;
}
@keyframes fall {
    0% { transform: translateY(0) rotate(0deg); }
    100% { transform: translateY(110vh) rotate(360deg); }
}

/* Container */
.container {
    padding: 40px 15px;
}

/* Name animation */
.name {
    font-size: 36px;
    font-weight: bold;
    color: #ff2f92;
    animation: heartbeat 1s infinite;
}

@keyframes heartbeat {
    0%, 100% { transform: scale(1); text-shadow: 0 0 5px #ff9acb; }
    50% { transform: scale(1.2); text-shadow: 0 0 20px #ff2f92; }
}

/* Typewriter effect */
.subtitle {
    margin-top: 8px;
    font-size: 20px;
    overflow: hidden;
    border-right: .15em solid #ff2f92;
    white-space: nowrap;
    width: 0;
    animation: typing 3s steps(30) forwards, blink .75s step-end infinite;
}

@keyframes typing { from { width: 0; } to { width: 22em; } }
@keyframes blink { 50% { border-color: transparent; } }

/* Photos */
.photos {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin: 25px 0;
    flex-wrap: wrap;
}
.photos img {
    width: 160px;
    height: 210px;
    object-fit: cover;
    border-radius: 15px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.5);
    transition: transform 0.3s;
}
.photos img:hover {
    transform: scale(1.1);
}

/* Card & button */
.card {
    background: rgba(0,0,0,0.6);
    border-radius: 16px;
    padding: 22px;
    max-width: 420px;
    margin: auto;
}
button {
    background: #ff2f92;
    color: white;
    border: none;
    padding: 12px 24px;
    font-size: 16px;
    border-radius: 25px;
    cursor: pointer;
    transition: transform 0.2s;
}
button:hover { transform: scale(1.1); }

/* Popup message */
#message {
    display: none;
    margin-top: 18px;
    line-height: 1.6;
    animation: fadein 1s forwards;
}
@keyframes fadein { from { opacity: 0; } to { opacity: 1; } }

/* Footer */
footer {
    margin-top: 35px;
    font-size: 14px;
    opacity: 0.8;
}
</style>
</head>

<body>
<div class="container">

    <div class="name">Mela Pyala Bacchaaa ❤️</div>
    <div class="subtitle">Happy New Year 2026 meri biwi jii ❤️</div>

    <div class="photos">
        <img src="photo1.jpg" alt="Our Memory 1">
        <img src="photo2.jpg" alt="Our Memory 2">
    </div>

    <div class="card">
        <p>Ek chhota sa surprise sirf aapke liye mela bacchaa💝</p>
        <button onclick="showMessage()">Click karo jaan</button>
        <div id="message">
            <p>
            Is naye saal me meri bas ek hi dua hai,  
            aap hamesha aise hi muskurati raho mela bacchaaa.
            </p>
            <p>
            Aap meri biwi hi nahi,  
            meri duniya, meri shanti aur meri sabse badi khushi ho bubuuuu.
            </p>
            <p>
            Happy New Year 2026 Mela Pyala Bacchaaa ❤️  
            Har saal, har pal, sirf aapke saath.
            </p>
        </div>
    </div>

    <footer>
        Made with aapke swami jii💖
    </footer>

</div>

<script>
/* Popup message */
function showMessage() {
    document.getElementById("message").style.display = "block";
}

/* Confetti creation */
for(let i=0;i<100;i++){
    let confetti = document.createElement('div');
    confetti.classList.add('confetti');
    confetti.style.left = Math.random() * window.innerWidth + 'px';
    confetti.style.backgroundColor = `hsl(${Math.random()*360}, 100%, 70%)`;
    confetti.style.animationDuration = (Math.random()*3+2) + 's';
    confetti.style.width = confetti.style.height = (Math.random()*8+5) + 'px';
    document.body.appendChild(confetti);
}
</script>
</body>
</html>

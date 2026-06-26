<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>🎁 Magic Gifts</title>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'Comic Sans MS', cursive, sans-serif;
    background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 50%, #a1c4fd 100%);
    min-height: 100vh;
    padding: 20px;
    overflow-x: hidden;
  }
  h1 {
    text-align: center;
    color: #fff;
    text-shadow: 3px 3px 0 #ff6b9d, 6px 6px 10px rgba(0,0,0,0.2);
    font-size: 3em;
    margin-bottom: 10px;
  }
  .subtitle {
    text-align: center;
    color: #fff;
    font-size: 1.3em;
    margin-bottom: 30px;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
  }
  .reset-btn {
    display: block;
    margin: 20px auto;
    padding: 12px 30px;
    font-size: 1.2em;
    background: #ff6b9d;
    color: white;
    border: none;
    border-radius: 50px;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: transform 0.2s;
  }
  .reset-btn:hover { transform: scale(1.1); }

  .gifts-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(110px, 1fr));
    gap: 20px;
    max-width: 1200px;
    margin: 0 auto;
  }

  .gift {
    position: relative;
    width: 100%;
    aspect-ratio: 1;
    cursor: pointer;
    transition: transform 0.3s;
  }
  .gift:hover { transform: scale(1.1) rotate(-3deg); }

  .gift-box {
    position: absolute;
    bottom: 0;
    left: 10%;
    width: 80%;
    height: 70%;
    border-radius: 8px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.25);
    animation: wiggle 2s ease-in-out infinite;
  }
  .gift-ribbon-v {
    position: absolute;
    left: 50%;
    top: 0;
    width: 15%;
    height: 100%;
    transform: translateX(-50%);
    background: rgba(255,255,255,0.7);
  }
  .gift-ribbon-h {
    position: absolute;
    top: 30%;
    left: 0;
    width: 100%;
    height: 15%;
    background: rgba(255,255,255,0.7);
  }
  .gift-bow {
    position: absolute;
    top: -15px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 2.5em;
    z-index: 2;
  }

  @keyframes wiggle {
    0%, 100% { transform: rotate(-2deg); }
    50% { transform: rotate(2deg); }
  }

  .gift.opened .gift-box,
  .gift.opened .gift-bow { display: none; }

  .sticker {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) scale(0) rotate(-20deg);
    width: 100%;
    height: 100%;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    font-weight: bold;
    color: white;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.4);
    box-shadow: 0 8px 25px rgba(0,0,0,0.3);
    padding: 10px;
    font-size: 0.95em;
    animation: pop 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55) forwards;
  }

  @keyframes pop {
    0% { transform: translate(-50%, -50%) scale(0) rotate(-180deg); }
    70% { transform: translate(-50%, -50%) scale(1.2) rotate(10deg); }
    100% { transform: translate(-50%, -50%) scale(1) rotate(0deg); }
  }

  .sparkle {
    position: absolute;
    pointer-events: none;
    font-size: 1.5em;
    animation: sparkle-fly 1s ease-out forwards;
  }
  @keyframes sparkle-fly {
    0% { opacity: 1; transform: translate(0,0) scale(0.5); }
    100% { opacity: 0; transform: translate(var(--tx), var(--ty)) scale(1.5); }
  }

  .score {
    text-align: center;
    font-size: 1.5em;
    color: #fff;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    margin-top: 20px;
  }
</style>
</head>
<body>

<h1>🎁 Open the Gifts! 🎁</h1>
<p class="subtitle">Click on each gift to reveal a surprise!</p>

<div class="gifts-grid" id="giftsGrid"></div>

<button class="reset-btn" onclick="resetGifts()">🔄 Play Again</button>
<div class="score">Opened: <span id="score">0</span> / <span id="total">0</span></div>

<script>
  const messages = [
    "Well done! ⭐", "Awesome! 🌟", "Great job! 👏",
    "Amazing! ✨", "Fantastic! 🎉", "Brilliant! 💡",
    "Super! 🚀", "Excellent! 🏆", "Perfect! 💯",
    "You rock! 🎸", "Wow! 😍", "Cool! 😎",
    "Yay! 🎊", "Hooray! 🥳", "Nice! 👍",
    "Bravo! 🎭", "Top! 🔝", "Star! ⭐",
    "Magic! 🪄", "Sweet! 🍬", "Superb! 🌈",
    "Genius! 🧠", "Hero! 🦸", "Champion! 🏅",
    "Legend! 👑", "Wonderful! 🌸", "Splendid! 💎",
    "Marvelous! 🎨", "Fabulous! 💃", "Terrific! 🎯"
  ];

  const colors = [
    "linear-gradient(135deg,#ff6b9d,#feca57)",
    "linear-gradient(135deg,#48dbfb,#0abde3)",
    "linear-gradient(135deg,#1dd1a1,#10ac84)",
    "linear-gradient(135deg,#f368e0,#ff9ff3)",
    "linear-gradient(135deg,#ff9f43,#ee5a24)",
    "linear-gradient(135deg,#5f27cd,#341f97)",
    "linear-gradient(135deg,#00d2d3,#01a3a4)",
    "linear-gradient(135deg,#ee5253,#c0392b)",
    "linear-gradient(135deg,#feca57,#ff6348)",
    "linear-gradient(135deg,#54a0ff,#2e86de)"
  ];

  const bowEmojis = ["🎀","🎁","🎀","🎁","🎀","🎁","🎀","🎁","🎀","🎁"];

  const grid = document.getElementById('giftsGrid');
  const GIFT_COUNT = 30;
  let opened = 0;

  function createGifts() {
    grid.innerHTML = '';
    opened = 0;
    document.getElementById('score').textContent = 0;
    document.getElementById('total').textContent = GIFT_COUNT;

    for (let i = 0; i < GIFT_COUNT; i++) {
      const gift = document.createElement('div');
      gift.className = 'gift';
      const color = colors[i % colors.length];
      const bow = bowEmojis[i % bowEmojis.length];

      gift.innerHTML = `
        <div class="gift-box" style="background:${color}">
          <div class="gift-ribbon-v"></div>
          <div class="gift-ribbon-h"></div>
        </div>
        <div class="gift-bow">${bow}</div>
      `;
      gift.addEventListener('click', () => openGift(gift, i));
      grid.appendChild(gift);
    }
  }

  function openGift(gift, index) {
    if (gift.classList.contains('opened')) return;
    gift.classList.add('opened');

    const msg = messages[index % messages.length];
    const color = colors[(index + 3) % colors.length];

    const sticker = document.createElement('div');
    sticker.className = 'sticker';
    sticker.style.background = color;
    sticker.textContent = msg;
    gift.appendChild(sticker);

    // sparkles
    for (let i = 0; i < 8; i++) {
      const s = document.createElement('div');
      s.className = 'sparkle';
      s.textContent = ['✨','⭐','💫','🌟','💖'][Math.floor(Math.random()*5)];
      const angle = (i / 8) * Math.PI * 2;
      const dist = 60 + Math.random() * 30;
      s.style.setProperty('--tx', Math.cos(angle) * dist + 'px');
      s.style.setProperty('--ty', Math.sin(angle) * dist + 'px');
      s.style.left = '50%';
      s.style.top = '50%';
      gift.appendChild(s);
      setTimeout(() => s.remove(), 1000);
    }

    opened++;
    document.getElementById('score').textContent = opened;

    if (opened === GIFT_COUNT) {
      setTimeout(() => alert('🎉 Congratulations! You opened all gifts! 🎉'), 500);
    }
  }

  function resetGifts() {
    createGifts();
  }

  createGifts();
</script>

</body>
</html>

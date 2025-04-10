<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>For Anushka</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom right, #ffe6f0, #fff0f5);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
    }
    .container {
      background-color: white;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
    }
    h1 {
      font-size: 24px;
      margin-bottom: 30px;
      color: #ff4d88;
    }
    button {
      padding: 12px 24px;
      font-size: 16px;
      border: none;
      border-radius: 10px;
      margin: 10px;
      cursor: pointer;
      transition: 0.3s;
    }
    #yesBtn {
      background-color: #ff4d88;
      color: white;
    }
    #noBtn {
      background-color: #ccc;
      color: #333;
      position: absolute;
    }
    #kittenContainer {
      margin-top: 20px;
      display: none;
    }
    #kittenContainer img {
      width: 200px;
      border-radius: 15px;
    }
    #kittenMessage {
      margin-top: 10px;
      font-size: 18px;
      color: #ff4d88;
    }
  </style>
</head>
<body>
  <!-- Background music -->
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-sunny.mp3" type="audio/mpeg">
  </audio>

  <div class="container">
    <h1>Anushka, would you like to go on a date with me?</h1>
    <button id="yesBtn">Yes</button>
    <button id="noBtn">No</button>
    <div id="kittenContainer">
      <img src="https://media.giphy.com/media/JIX9t2j0ZTN9S/giphy.gif" alt="Cute Kitten">
      <div id="kittenMessage">Let's goo, baddie! Let's do it tomorrow — we’ll ball!</div>
    </div>
  </div>

  <script>
    const yesBtn = document.getElementById('yesBtn');
    const noBtn = document.getElementById('noBtn');
    const kittenContainer = document.getElementById('kittenContainer');

    yesBtn.addEventListener('click', () => {
      kittenContainer.style.display = 'block';
    });

    noBtn.addEventListener('mouseover', () => {
      const x = Math.floor(Math.random() * (window.innerWidth - 100));
      const y = Math.floor(Math.random() * (window.innerHeight - 50));
      noBtn.style.left = `${x}px`;
      noBtn.style.top = `${y}px`;
    });
  </script>
</body>
</html>


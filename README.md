# Geometry-dash<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Geometry Dash | Alexx743</title>

  <style>
    body {
      margin: 0;
      background: #111;
      color: white;
      font-family: Arial, sans-serif;
      text-align: center;
    }

    h2 {
      margin: 10px 0;
    }

    .topnav {
      display: flex;
      justify-content: center;
      gap: 8px;
      padding: 8px;
      background: #222;
    }

    .topnav button {
      background: #444;
      color: white;
      border: none;
      padding: 8px 12px;
      cursor: pointer;
      border-radius: 4px;
    }

    iframe {
      width: 95vw;
      height: 75vh;
      border: none;
      margin-top: 10px;
      background: black;
    }

    .fullscreen {
      margin: 10px;
      padding: 10px 16px;
      background: #0a84ff;
      border: none;
      color: white;
      cursor: pointer;
      border-radius: 4px;
    }
  </style>
</head>

<body>

<h2>Geometry Dash</h2>

<div class="topnav">
  <button onclick="location.href='index.html'">Home</button>
  <button onclick="location.href='games.html'">Games</button>
  <button onclick="location.href='Apps.html'">Apps</button>
</div>

<iframe
  id="game"
  src="https://geometrydashlite.io/"
  tabindex="0">
</iframe>

<br>

<button class="fullscreen" onclick="goFullscreen()">
  Fullscreen
</button>

<script>
  function goFullscreen() {
    const iframe = document.getElementById("game");
    iframe.style.position = "fixed";
    iframe.style.top = "0";
    iframe.style.left = "0";
    iframe.style.width = "100vw";
    iframe.style.height = "100vh";
    iframe.style.zIndex = "9999";
    iframe.focus();
  }

  window.onload = () => {
    document.getElementById("game").focus();
  };
</script>

</body>
</html>

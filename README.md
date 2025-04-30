<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Deportes en Vivo</title>
  <style>
    body {
      background-color: #000;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #111;
      padding: 20px;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
      color: #00ffcc;
    }
    nav {
      background-color: #222;
      padding: 10px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav button {
      margin: 5px;
      padding: 10px 20px;
      background-color: #00ffcc;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      color: black;
      font-weight: bold;
    }
    nav button:hover {
      background-color: #00ddaa;
    }
    .iframe-container {
      display: flex;
      justify-content: center;
      padding: 20px;
    }
    iframe {
      width: 80%;
      height: 480px;
      border: none;
    }
  </style>
</head>
<body>

  <header>
    🏟️ Deportes en Vivo 2025
  </header>

  <nav>
    <button onclick="cambiarCanal('https://topembed.pw/channel/ESPN[Latin%20America]')">ESPN</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/TNT_Sports[Latin%20America]')">TNT Sports</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/FOX_Sports[Latin%20America]')">FOX Sports</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/NBATV[USA]')">NBA TV</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/GOLFChannel[USA]')">GOLF Channel</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/ESPNKnockOut[Latin%20America]')">ESPN KnockOut</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/TennisChannel[USA]')">Tennis Channel</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/ArenaPremium1[Serbia]')">Arena Premium 1</button>
    <button onclick="cambiarCanal('https://topembed.pw/channel/ESPNExtra[Latin%20America]')">ESPN Extra</button>
  </nav>

  <div class="iframe-container">
    <iframe id="tvFrame" src="https://topembed.pw/channel/ESPN[Latin%20America]" allow="encrypted-media" allowfullscreen></iframe>
  </div>

  <script>
    function cambiarCanal(url) {
      document.getElementById("tvFrame").src = url;
    }
  </script>

</body>
</html>

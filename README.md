
<!DOCTYPE html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>A Minha Primeira Experiência AR</title>

  <script src="https://aframe.io/releases/1.4.2/aframe.min.js"></script>
  <script src="https://cdn.jsdelivr.net/gh/AR-js-org/AR.js@3.4.5/aframe/build/aframe-ar.js"></script>
</head>

<body style="margin: 0; overflow: hidden;">
  <a-scene embedded arjs="sourceType: webcam;">

    <a-marker preset="hiro">
      <a-box
        position="0 0.5 0"
        material="color: #6C63FF;"
        animation="property: rotation; to: 0 360 0; loop: true; dur: 4000">
      </a-box>

      <a-text
        value="A minha primeira experiencia AR!"
        position="-1.2 1.2 0"
        rotation="-90 0 0"
        color="#FFFFFF"
        align="center"
        width="3">
      </a-text>
    </a-marker>

    <a-entity camera></a-entity>
  </a-scene>
</body>
</html>

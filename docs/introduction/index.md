<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Clase 1 - Mi primera escena A-Frame</title>
  <!-- Cargamos la librería oficial de A-Frame -->
  <script src="https://aframe.io/releases/1.8.0/aframe.min.js"></script>
</head>
<body>

  <!-- Contenedor principal de la escena 3D -->
  <a-scene>

    <!-- 1. Cubo celeste -->
    <!-- Posición: X = -1, Y = 0.5, Z = -3 (metros) -->
    <!-- Rotación en Y = 45 grados -->
    <a-box 
      position="-1 0.5 -3" 
      rotation="0 45 0" 
      color="#4CC3D9">
    </a-box>

    <!-- 2. Esfera roja -->
    <!-- Radio de 1.25 metros -->
    <a-sphere 
      position="0 1.25 -5" 
      radius="1.25" 
      color="#EF2D5E">
    </a-sphere>

    <!-- 3. Cilindro amarillo -->
    <a-cylinder 
      position="1 0.75 -3" 
      radius="0.5" 
      height="1.5" 
      color="#FFC65D">
    </a-cylinder>

    <!-- 4. Plano/Piso verde -->
    <!-- Se rota -90° en X para acostarlo horizontalmente -->
    <a-plane 
      position="0 0 -4" 
      rotation="-90 0 0" 
      width="4" 
      height="4" 
      color="#7BC8A4">
    </a-plane>

    <!-- 5. Fondo / Cielo de la escena -->
    <a-sky color="#ECECEC"></a-sky>

    <!-- 6. Cámara y controles por defecto (Opcional) -->
    <!-- Si no se especifica, A-Frame la coloca automáticamente en (0, 1.6, 0) -->
    <a-entity camera look-controls wasd-controls position="0 1.6 0"></a-entity>

  </a-scene>

</body>
</html>

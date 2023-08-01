<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Imajinasi Bunga Bergerak</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="flower-container">
    <div class="flower"></div>
  </div>
</body>
</html>
body, html {
  height: 100%;
  margin: 0;
  overflow: hidden;
}

.flower-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  background-color: #f0f0f0;
  overflow: hidden;
}

.flower {
  width: 100px;
  height: 100px;
  background-image: url("path/to/your-flower-image.png");
  background-size: cover;
  animation: moveFlower 4s ease-in-out infinite;
}

@keyframes moveFlower {
  0%, 100% {
    transform: translate(0, 0);
  }
  50% {
    transform: translate(50px, -50px);
  }
}

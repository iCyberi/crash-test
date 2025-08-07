<!DOCTYPE html>
<html>
<head>
  <title>iPhone Freeze Test</title>
</head>
<body>
  <h1>Freeze Test</h1>
  <p>If your browser freezes, the test worked.</p>

  <script>
    // Infinite loop to cause heavy CPU usage
    setTimeout(function loop() {
      for (let i = 0; i < 1e8; i++) {
        let a = new Array(10000).fill("Freeze!");
      }
      setTimeout(loop, 0);
    }, 0);
  </script>
</body>
</html>

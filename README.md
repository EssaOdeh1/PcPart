<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>QR Code for Camera</title>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
  <style>
    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      font-family: Arial, sans-serif;
    }
    h1 {
      margin-bottom: 20px;
    }
    #qrcode {
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>Scan to Open Camera</h1>
  <div id="qrcode"></div>
  <script>
    // URL to open the camera functionality
    const cameraPageUrl = "https://your-web-app.com/camera";

    // Generate the QR code
    new QRCode(document.getElementById("qrcode"), {
      text: cameraPageUrl,
      width: 256,
      height: 256,
    });
  </script>
</body>
</html>

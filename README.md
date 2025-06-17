<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Redireccionando a WhatsApp...</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: url('https://cdn.pixabay.com/photo/2020/09/21/09/57/casino-5589154_1280.jpg') no-repeat center center fixed;
      background-size: cover;
      font-family: Arial, sans-serif;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
      text-align: center;
    }

    .spinner {
      margin-top: 20px;
      width: 50px;
      height: 50px;
      border: 5px solid rgba(255, 255, 255, 0.3);
      border-top: 5px solid #25D366;
      border-radius: 50%;
      animation: spin 1s linear infinite;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .whatsapp-icon {
      font-size: 60px;
      color: #25D366;
      margin-bottom: 10px;
    }
  </style>
  <script>
    setTimeout(() => {
      const numero = "541134413881"; // Código de país + número (sin 0 ni +)
      const mensaje = encodeURIComponent("Quisiera un usu4rio con mi 30% de bonificación");
      const url = `https://wa.me/${numero}?text=${mensaje}`;
      window.location.href = url;
    }, 2000); // Espera 2 segundos
  </script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body>
  <i class="fab fa-whatsapp whatsapp-icon"></i>
  <h1>Estamos conectándote con un asesor de WhatsApp...</h1>
  <div class="spinner"></div>
</body>
</html>

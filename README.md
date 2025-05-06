<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>lovelovelove!!!</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      background: linear-gradient(135deg, #ffd6e6, #ffe6f0);
      background-size: 400% 400%;
      animation: backgroundGradient 20s ease infinite;
      color: #4a0033;
      font-family: Arial, sans-serif;
      font-size: 14px;
      font-weight: bold;
      font-style: italic;
      text-align: center;
      overflow-x: hidden;
      position: relative;
      transition: background 1s ease, color 0.5s ease;
    }

    @keyframes backgroundGradient {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .bienvenida {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: #ffe6f0;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      z-index: 999;
      animation: fadeInText 2s ease;
    }

    .bienvenida h1 {
      font-size: 2em;
      margin-bottom: 20px;
    }

    .btn-loviu {
      padding: 12px 24px;
      font-size: 1.2em;
      border: none;
      border-radius: 30px;
      background-color: #ff66a3;
      color: white;
      cursor: pointer;
      font-style: italic;
      font-weight: bold;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      transition: transform 0.3s ease, background-color 0.3s ease;
    }

    .btn-loviu:hover {
      transform: scale(1.1);
      background-color: #ff3385;
    }

    .contenido {
      display: none;
      animation: fadeInText 2s ease;
    }

    @keyframes fadeInText {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .mensaje, .mensaje-final {
      padding: 30px 20px 10px;
      max-width: 800px;
      margin: 0 auto;
      z-index: 2;
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 1s ease, transform 1s ease;
    }

    .mensaje.visible, .mensaje-final.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .mensaje-final {
      margin-bottom: 80px;
    }

    .collage {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      gap: 15px;
      padding: 20px;
      z-index: 2;
    }

    .collage img {
      width: 300px;
      max-width: 90%;
      height: auto;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 1s ease, transform 1s ease;
    }

    .collage img.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .collage img:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
    }

    .heart {
      position: fixed;
      top: 100%;
      color: #ff3366;
      font-size: 20px;
      animation: floatHeart 10s linear infinite;
      opacity: 0.8;
      z-index: 1;
    }

    @keyframes floatHeart {
      0% {
        transform: translateY(0) translateX(0) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-120vh) translateX(-30px) rotate(360deg);
        opacity: 0;
      }
    }

    .mensaje-frase {
      text-align: center;
      font-size: 1.5em;
      margin: 20px 0;
      font-style: italic;
      font-weight: bold;
      color: #4a0033;
      display: block;
      width: 100%;
      justify-content: center;
    }

    /* Estilo para la imagen en el mensaje sorpresa */
    #mensaje-sorpresa {
      display: none;
      margin-top: 20px;
      font-size: 1.2em;
      opacity: 0;
      transition: opacity 1s ease;
      text-align: center; /* Centrado de la frase */
    }

    #mensaje-sorpresa img {
      width: 80%;  /* Ajusta el tamaño de la imagen */
      max-width: 400px;  /* Limita el tamaño máximo */
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      margin-bottom: 20px;
    }

    @media (max-width: 600px) {
      .mensaje, .mensaje-final {
        padding: 20px 15px;
        font-size: 13px;
      }

      .collage {
        flex-direction: column;
        gap: 10px;
      }

      .collage img {
        width: 90%;
      }

      .mensaje-final {
        margin-bottom: 100px;
      }
    }
  </style>
</head>
<body>

  <!-- Pantalla de bienvenida -->
  <div class="bienvenida" id="bienvenida">
    <h1>olii</h1>
    <button class="btn-loviu" onclick="mostrarContenido()">loviu^^</button>
  </div>

  <!-- Contenido principal -->
  <div class="contenido" id="contenido">

    <!-- Mensaje especial -->
    <div class="mensaje">
      Todas las canciones de este álbum tan hermoso me hacen recordarte, pensar en ti y saber la manera tan especial en la que te amo y como me haces sentir.  
      Cada canción es una carta al amor, cada canción es linda y transmite un lindo mensaje.  
      Te amo tanto mi bella, espero lo disfrutes.  
      <br><br>
      Hace que recuerde cada momento bello que hemos compartido juntos, cada día, cada abrazo, cada beso.  
      Todo lo lindo que hemos hecho juntos y así como también hemos pasado momentos hermosos, en su mayoría también hemos pasado momentos difíciles.  
      Más sin embargo, siempre superamos las cosas juntos porque de eso se trata.  
      Nos faltan tantas cosas por hacer, tantas cosas planeadas por cumplir.  
      Sos lo más lindo que la vida y Dios pudo poner en mi camino.  
      Te amo infinitamente, mi bella &lt;3  
      <br><br>
      GIRL, I'M SO IN LOVE WITH YOU &hearts;
    </div>

    <!-- Collage -->
    <div class="collage">
      <img src="IMg_2701.JPEG" alt="Foto 1">
      <img src="img_2706.jpeg" alt="Foto 2">
      <img src="IMG_2954.JPEG" alt="Foto 3">
      <img src="IMG_3479.JPEG" alt="Foto 4">
      <img src="IMG_4052.JPEG" alt="Foto 5">
      <img src="IMG_4062.JPEG" alt="Foto 6">
      <img src="IMG_3729.JPEG" alt="Foto 7">
      <div class="mensaje-frase">
        YOU REMIND ME OF THE COLOR BLUE^^
      </div>
      <img src="IMG_4468.JPEG" alt="Foto 8">
      <img src="IMG_5042.JPEG" alt="Foto 9">
      <img src="IMG_4475.JPEG" alt="Foto 10">
      <img src="IMG_0733.JPEG" alt="foto 11">
      <img src="IMG_1215.JPEG" alt="foto 12">
      <img src="IMG_1271.JPEG" alt="foto 13">
      <img src="IMG_1804.JPEG" alt="foto 14">
    </div>

    <!-- Mensaje final -->
    <div class="mensaje-final">
      Hay tantas historias, una distinta por cada foto.  
      Cada canción un mensaje diferente, cada mensaje un sentimiento distinto y cada sentimiento es bello.  
      Sos lo más lindo que puedo tener.  
      Benditas mis manos que pueden tocarte, agradecidos mis ojos que pueden apreciar y admirar tu belleza que alegra mis días. 
      <br><br>
      Tantas cosas lindas que hemos hecho juntos, tantos momentos gratificantes y llenos de amor.  
      La vida es bella cuando estoy junto a ti, haces que todo tenga sentido.  
      Me haces estar cuerdo y me motivas a seguir adelante en todo.  
      Sos la luz de mis ojos y la alegría de mis días. 
      <br><br>
      GRACIAS POR TANTO Y PERDÓN POR TAN POCO, TE AMO INFINITAMENTE &lt;3
      <br><br>

      <!-- Botón sorpresa -->
      <button class="btn-loviu" onclick="mostrarSorpresa()">Toca aquí para ver algo kul jijijijij</button>

      <!-- Mensaje sorpresa -->
      <div id="mensaje-sorpresa">
        <img src="IMG_2721.JPEG" alt="foto 1">
        <br><br>
        Sos el amor de mi vida.  
        Estoy completamente seguro de que Dios te puso en mi camino por una razón,  
        y no hay día que no agradezca por tenerte.    
        ¡Gracias por existir, mi amol! &lt;3
      </div>
    </div>
  </div>

  <!-- Script -->
  <script>
    const createHeart = () => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = 12 + Math.random() * 24 + "px";
      heart.style.animationDuration = (8 + Math.random() * 4) + "s";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 12000);
    };
    setInterval(createHeart, 500);

    function mostrarContenido() {
      document.getElementById("bienvenida").style.display = "none";
      document.getElementById("contenido").style.display = "block";

      const audio = document.createElement('audio');
      audio.src = "Mac Miller - Congratulations Instrumental (VIOLIN & PIANO) ❦ - b.mp3";
      audio.loop = true;
      audio.autoplay = true;
      audio.style.display = "none";
      document.body.appendChild(audio);
      audio.play().catch(e => console.log("Audio bloqueado por el navegador:", e));
    }

    function mostrarSorpresa() {
      const sorpresa = document.getElementById("mensaje-sorpresa");
      sorpresa.style.display = "block";
      setTimeout(() => {
        sorpresa.style.opacity = 1;
      }, 10);
    }

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('.collage img, .mensaje, .mensaje-final').forEach(el => {
      observer.observe(el);
    });
  </script>
</body>
</html>

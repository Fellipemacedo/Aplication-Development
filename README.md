<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Travel Destinations</title>
  <style>
    /* Optional styles for page layout */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #cfe2f3; /* Light blue color */
    }
    .container {
      max-width: 900px;
      margin: 20px auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    h1 {
      text-align: center;
      font-family: 'Lucida Handwriting', sans-serif; /* Gothic style font */
    }
    .destino {
      display: flex;
      justify-content: space-between;
      margin-bottom: 20px;
    }
    .destino div {
      width: 45%; /* Distribute images evenly */
    }
    .destino img {
      width: 100%;
      height: auto;
      cursor: pointer;
      transition: transform 0.3s ease;
      border-radius: 10px; /* Rounded borders */
    }
    .destino img:hover {
      transform: scale(1.1);
    }
    .titulo {
      text-align: center;
      margin-top: 20px;
      font-size: 20px;
    }
    .btn-container {
      text-align: center;
      margin-top: 30px;
    }
    .btn-container a {
      display: inline-block;
      margin: 0 50px;
    }
    .btn-container img {
      width: 200px;
      height: auto;
    }
  </style>
</head>
<body>


<div class="container">
  <h1>Travel+</h1> 
  <div class="destinos">
    <div class="destino">
      <div>
        <img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\Paris_01.jpg" alt="Paris, France" onclick="openModal('Paris, França', 'Paris is the capital of France and one of the most popular tourist destinations in the world. Known as the City of Light, it is famous for its iconic landmarks such as the Eiffel Tower and the Louvre Museum.')">
        <p class="titulo">Paris, França</p>
      </div>
      <div>
        <img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\Tókio_03.jpg" alt="Tokyo, Japan" onclick="openModal('Tóquio, Japão', 'Tokyo is the capital of Japan and one of the most vibrant and exciting cities in the world. It\'s a unique blend of tradition and modernity, with an incredible variety of cultural, gastronomic, and entertainment experiences.')">
        <p class="titulo">Tóquio, Japão</p>
      </div>
    </div>
    <div class="destino">
      <div>
        <img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\RiodeJaneiro_02.jpg" alt="Rio de Janeiro, Brazil" onclick="openModal('Rio de Janeiro, Brasil', 'Rio de Janeiro is known for its stunning beaches like Copacabana and Ipanema, its iconic urban landscape with the Sugarloaf Mountain and the Christ the Redeemer, and its vibrant and festive energy.')">
        <p class="titulo">Rio de Janeiro, Brasil</p>
      </div>
      <div>
        <img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\Sidney.jpeg" alt="Sydney, Australia" onclick="openModal('Sydney, Austrália', 'Sydney is one of Australia\'s most famous cities, known for its beautiful Opera House, its iconic Sydney Harbour Bridge, its stunning beaches, and its vibrant cultural and gastronomic scene.')">
        <p class="titulo">Sydney, Austrália</p>
      </div>
    </div>
  </div>
</div>

<div class="btn-container">
    <a href="Form1.html"><img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\Reserv.png" alt="Make your reservation"></a>
    <a href="nm.html"><img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\graph.jpg" alt="See the Graph"></a>
    <a href="Login1.html"><img src="C:\Users\User\Desktop\College IT\2 Term\Storage database\Final Project\Proj.WebTravel+\login.jpg" alt="Login"></a>
</div>



<!-- Modal -->
<div id="modal" class="modal">
  <div class="modal-content">
    <span class="close" onclick="closeModal()">&times;</span>
    <h2 id="modal-title"></h2>
    <p id="modal-description"></p>
  </div>
</div>

<script>
  function openModal(title, description) {
    document.getElementById("modal-title").innerHTML = title;
    document.getElementById("modal-description").innerHTML = description;
    document.getElementById("modal").style.display = "block";
  }

  function closeModal() {
    document.getElementById("modal").style.display = "none";
  }
</script>

</body>
</html>

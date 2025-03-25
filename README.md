<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfólio Modelo</title>
  <!-- Fonte do Google Fonts para dar estilo de revista -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Lora:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Lora', serif;
      background-color: #f5f5f5;
      color: #333;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }
    .container {
      text-align: center;
      max-width: 600px;
      width: 100%;
      background-color: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 15px rgb(255, 0, 0);
      opacity: 0;
      transform: translateY(50px);
      animation: fadeInUp 1s forwards; /* Animação para o conteúdo */
    }
    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    h1 {
      font-family: 'Playfair Display', serif;
      font-size: 4em;
      font-weight: 700;
      cursor: pointer;
      transition: color 0.3s ease;
      letter-spacing: 2px;
      opacity: 0;
      animation: fadeIn 1.5s forwards;
    }
    h1:hover {
      color: #e74c3c;
    }
    @keyframes fadeIn {
      to {
        opacity: 1;
      }
    }
    .options {
      margin-top: 30px;
      display: none;
      opacity: 0;
      animation: fadeInOptions 1.5s forwards;
    }
    @keyframes fadeInOptions {
      to {
        opacity: 1;
      }
    }
    .options a {
      display: inline-block;
      margin: 10px 20px;
      font-family: 'Lora', serif;
      font-size: 1.4em;
      color: #333;
      text-decoration: none;
      transition: color 0.3s ease;
      letter-spacing: 1px;
    }
    .options a:hover {
      color: #e74c3c;
    }
    .content {
      display: none;
      margin-top: 20px;
      max-height: 70vh; /* Limita a altura da seção */
      overflow-y: auto; /* Permite o scroll se o conteúdo for maior que a altura */
    }
    .content.active {
      display: block;
    }
    .back-button {
      display: inline-block;
      margin-top: 20px;
      font-family: 'Lora', serif;
      font-size: 1.2em;
      color: #333;
      text-decoration: none;
      transition: color 0.3s ease;
      letter-spacing: 1px;
    }
    .back-button:hover {
      color: #e74c3c;
    }

    /* Estilos para la galería de fotos */
    .photo-gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); /* Hacer una cuadrícula de fotos */
      gap: 15px;
      padding: 20px;
    }
    .photo-gallery img {
      width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
    }
    .photo-gallery img:hover {
      transform: scale(1.05); /* Efecto de agrandamiento de imagen al pasar el ratón */
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Solo se muestra el nombre al inicio -->
    <h1 id="model-name" onclick="toggleOptions()">Alorha</h1>

    <!-- Opciones (inicialmente ocultas) -->
    <div class="options" id="options">
      <a href="#" onclick="showContent('bio')">Biografia</a>
      <a href="#" onclick="showContent('contact')">Contato</a>
      <a href="#" onclick="showContent('photos')">Fotos</a>
    </div>

    <!-- Conteúdo de cada seção -->
    <div id="bio" class="content">
      <h2>Biografia</h2>
      <p>
        Eu sou Alorha, sou moradora do complexo da maré e tenho 19 anos de idade, sou artista independente desde que eu me entendo por pessoa, sempre gostei de estar envolvida com a arte.
        Eu não entendia o que eu queria é nem sabia o que era ser artista, até que eu tive meu primeiro contato com o teatro em um projeto comunitário e aonde eu também tive contato com a palhaçaria, e foi minha primeira paixão que eu lembro que quando eu me via fantasiada e caracterizada me sentia uma celebridade, mas infelizmente o projeto só tinha a duração de 1 ano no local aonde eu morava.
        Então é de se imaginar que eu tenha ficado bem chateada com o encerramento do projeto, até que eu acabei conhecendo um outro projeto comunitário pertinho de casa.
        É óbvio que eu pedir para minha mãe pra me inscrever mas já era tarde demais pois as vagas já estavam todas preenchidas e então tive que esperar um ano para fazer parte do projeto de teatro. 
        No ano seguinte, eu já não via a hora de me inscrever e eu lembro como se fosse hoje.
        Foi no ano de 2018, a maré estava em um período de confrontos policiais muito em alta, minha mãe é claro ficava preocupada de deixar eu ir sozinha mas como era do ladinho de casa ela decidiu me inscrever, também ela já conhecia o espaço, pois eu já pegava livros na biblioteca que existe até hoje, fica no museu da maré ao lado do morro do timbau.
        Ao entrar para o projeto percebi que tinham pessoas bem mais velhas que eu e me sentia quase uma celebridade por ter esse contato.
        Eu no início não entendia muito sobre teatro até que eu tive meu primeiro contato com o festival de cenas, aonde eu teria que produzir toda a cena com o meu grupo. Foi uma experiência que exigiu muita paciência e muita dedicação, eu também nunca gostei de deixar nada pela metade, então fui até o final.
        Enfim já fazem 5 anos que estou nesse projeto que vem me ensinando muito e principalmente como a lidar com as diversidades de pensamentos e ideias.
        Mas não foi só lá que eu adquiri conhecimento a vida também me ensinou muito e me ensinou o quanto a vida é dura.
        Sou uma mulher, trans, preta, periférica e não vejo isso como algo ruim não, amo a minha identidade sei quem sou e sei que não dar para romantinzar o fato de ser a classe que mais sofre com o sistema e viver em um país que mais mata pessoas trans do mundo. Eu não tenho medo desse mundo e muito menos do sistema a voz que ecoa dentro de mim vem de uma ancestralidade que já vem a luta a muito anos e nunca paramos, e prova viva que eu tenho é que eu estou viva, viva para lutar viva pra saborear o que vida tem de melhor e viva para questionar sobre o que a de pior.
        O melhor que eu tenho hoje é o meu corpo presente, que estuda, investiga, escuta, fala, sente. Sinto que estou caminhando para ser uma pessoa melhor e melhorando a cada dia mais.
        Eu hoje já fiz vários trabalhos comunitários, cursos, participações em clipes, figuração, tive também contato com áudio visual, desfile de moda, categoria baby vogue na ballroom Rio, no total partirei de três festivais de cenas curtas, quatro espetáculos e uma apresentação homenagem.</p>
      <a href="#" class="back-button" onclick="backToMain()">Voltar ao início</a>
    </div>
    <div id="contact" class="content">
      <h2>Contato</h2>
      <p>E-mail:
         Celular:
      </p>
      <a href="#" class="back-button" onclick="backToMain()">Voltar ao início</a>
    </div>
    <div id="photos" class="content">
      <h2>Fotos</h2>

      <!-- Galería de fotos -->
      <div class="photo-gallery">
        <!-- Aquí puedes agregar las imágenes de la modelo -->
        <img src="imagenes/1.jpg" alt="Foto 1">
        <img src="imagenes/2.jpg" alt="Foto 2">
        <img src="imagenes/3.jpg" alt="Foto 3">
        <img src="imagenes/4.jpg" alt="Foto 4">
        <img src="imagenes/5.jpg" alt="Foto 5">
        <img src="imagenes/6.jpg" alt="Foto 6">
      </div>

      <a href="#" class="back-button" onclick="backToMain()">Voltar ao início</a>
    </div>
  </div>

  <script>
    // Função para alternar entre mostrar as opções e a seção de fotos
    function toggleOptions() {
      const options = document.getElementById('options');
      const modelName = document.getElementById('model-name');

      // Mostrar las opciones y ocultar el nombre de la modelo
      if (options.style.display === 'none' || options.style.display === '') {
        options.style.display = 'block'; // Mostrar las opciones
        modelName.style.display = 'none'; // Ocultar el nombre
      } else {
        options.style.display = 'none'; // Ocultar las opciones
        modelName.style.display = 'block'; // Mostrar el nombre
      }
    }

    // Función para mostrar el contenido de cada sección
    function showContent(section) {
      // Ocultar todo el contenido
      const contents = document.querySelectorAll('.content');
      contents.forEach(content => content.classList.remove('active'));

      // Mostrar el contenido de la sección seleccionada
      document.getElementById(section).classList.add('active');
    }

    // Función para volver a la página inicial
    function backToMain() {
      const options = document.getElementById('options');
      const contents = document.querySelectorAll('.content');
      const modelName = document.getElementById('model-name');

      // Ocultar todas las secciones y mostrar el nombre de la modelo
      contents.forEach(content => content.classList.remove('active'));
      options.style.display = 'none';
      modelName.style.display = 'block';
    }
  </script>
</body>
</html>

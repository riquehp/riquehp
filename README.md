<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nosso Casamento</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Estilos básicos */
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            margin: 0;
            padding: 20px;
        }

        nav {
            background-color: #001f3f;
            padding: 15px;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
            padding: 10px 20px;
            background-color: #003366; /* Azul mais escuro */
            border-radius: 8px;
            border: 2px solid #002244;
        }

        nav ul li a:hover {
            background-color: #002244; /* Fundo ao passar o mouse */
        }

        h2 {
            color: #001f3f;
            text-align: center;
            margin-top: 30px;
        }

        section {
            display: none;
            margin: 30px 0;
        }

        section.active {
            display: block;
        }

        p, ul {
            font-size: 18px;
            text-align: center;
        }

        iframe {
            display: block;
            margin: 0 auto;
            border: 0;
        }

        /* Paleta de cores visual */
        .color-box {
            display: inline-block;
            width: 100px;
            height: 100px;
            margin: 10px;
            border: 1px solid #ccc;
        }

        /* Fundo azul claro para a seção "Nossa História" */
        #nossa-historia {
            background: linear-gradient(to bottom right, #e0f7fa, #b3e5fc);
            padding: 20px;
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <!-- Navegação entre as abas -->
    <nav>
        <ul>
            <li><a href="#" onclick="showSection('nossa-historia')">Nossa História</a></li>
            <li><a href="#" onclick="showSection('data-e-local')">Data & Local</a></li>
            <li><a href="#" onclick="showSection('presentes')">Sugestões de Presentes</a></li>
            <li><a href="#" onclick="showSection('cores')">Padrinhos</a></li>
        </ul>
    </nav>

    <!-- Seção de História -->
    <section id="nossa-historia" class="active">
        <h2>Nossa História</h2>
        
        <p><strong>Henrique:</strong></p>
        <p>Tudo começou no dia 28 de abril. Eu estava curtindo um pagode e, no meio da música, decidi mandar uma mensagem para a Aline. O que eu não esperava era que, logo depois de enviar a mensagem, meu celular quebraria! Fiquei sem saber se ela tinha respondido ou não. O suspense durou até conseguir resolver o problema, e foi então que descobri a resposta dela, abrindo caminho para uma história de amor que só cresceria com o tempo.</p>
        
        <br>
        
        <p><strong>Aline:</strong></p>
        <p>Estava eu num dia comum, mais precisamente dia 28 de abril, em uma lanchonete com os amigos, quando vejo uma notificação de mensagem do Henrique. Não sabia muito bem como responder, até que na madrugada chega outra mensagem falando que ele tinha quebrado o celular, em tom brincalhão, que abriu caminho para uma conversa leve, que mudaria pra sempre nossas vidas, dando início a nossa história de amor..</p>

        <img src="foto_primeiro_encontro.jpg" alt="Nosso primeiro encontro" width="300" style="display: block; margin: 0 auto;">
    </section>

    <!-- Seção de Data & Local -->
    <section id="data-e-local">
        <h2>Data & Local</h2>
        <p>A cerimônia será realizada no dia <strong>27 de junho de 2025</strong>, às <strong>17h</strong>, no <strong>Espaço Jardim Encantado</strong>, em <strong>Salto Grande - SP</strong>.</p>
        <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d14633.961651858247!2d-50.011105!3d-22.897917!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94bf51840f93d141%3A0x2209f83b9d85a207!2sSalto%20Grande%20-%20SP!5e0!3m2!1spt-BR!2sbr!4v1663953170989!5m2!1spt-BR!2sbr" width="600" height="450"></iframe>
    </section>

    <!-- Seção de Sugestões de Presentes -->
    <section id="presentes">
        <h2>Sugestões de Presentes</h2>
        <p>Se desejar nos presentear, veja nossas listas de presentes ou contribua com nossa lua de mel!</p>
        <ul>
            <li><a href="https://www.lista-de-presentes.com">Lista de Presentes - Loja X</a></li>
            <li><a href="https://www.vaquinha.com.br">Contribua para a Lua de Mel</a></li>
        </ul>
    </section>

    <!-- Seção de Paleta de Cores -->
    <section id="cores">
        <h2>Paleta de traje para os padrinho</h2>
        <p>Veja os tons de azul claro sugeridos para o nosso casamento:</p>
        
        <div class="color-box" style="background-color: #e0f7fa;"></div>
        <div class="color-box" style="background-color: #b3e5fc;"></div>
        <div class="color-box" style="background-color: #81d4fa;"></div>
        <div class="color-box" style="background-color: #4fc3f7;"></div>
        <div class="color-box" style="background-color: #29b6f6;"></div>
        <div class="color-box" style="background-color: #03a9f4;"></div>
        <div class="color-box" style="background-color: #0288d1;"></div>
    </section>

    <script>
        // Função para mostrar a seção selecionada e esconder as outras
        function showSection(sectionId) {
            // Ocultar todas as seções
            var sections = document.querySelectorAll('section');
            sections.forEach(function(section) {
                section.classList.remove('active');
            });

            // Mostrar a seção selecionada
            var sectionToShow = document.getElementById(sectionId);
            sectionToShow.classList.add('active');
        }
    </script>
</body>
</html>

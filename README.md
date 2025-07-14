<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proposta de Sequência de E-mails | CEDIN</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lato:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #007bff; /* Azul primário */
            --secondary-color: #6c757d; /* Cinza secundário */
            --background-color: #f8f9fa; /* Fundo claro */
            --card-bg: #ffffff; /* Fundo do card */
            --note-bg: #fffbe6; /* Fundo das notas */
            --text-color: #343a40;
            --border-color: #dee2e6;
            --cta-color: #4CAF50;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Lato', sans-serif;
            background-color: var(--background-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background-color: var(--card-bg);
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            overflow: hidden;
        }

        header {
            padding: 20px 30px;
            background-color: var(--primary-color);
            color: white;
            text-align: center;
        }

        header h1 {
            margin-bottom: 5px;
        }

        .nav-bar {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            padding: 10px;
            background-color: #f1f1f1;
            border-bottom: 1px solid var(--border-color);
        }

        .nav-bar button {
            background-color: transparent;
            border: 1px solid var(--secondary-color);
            color: var(--secondary-color);
            padding: 8px 12px;
            margin: 5px;
            border-radius: 5px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .nav-bar button.active,
        .nav-bar button:hover {
            background-color: var(--secondary-color);
            color: white;
        }

        .slide {
            display: none;
            padding: 30px;
            animation: fadeIn 0.5s;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .slide-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 25px;
        }

        @media (min-width: 768px) {
            .slide-content {
                grid-template-columns: 3fr 2fr;
            }
        }

        .email-preview {
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 20px;
        }

        .email-header {
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 10px;
            margin-bottom: 15px;
        }
        
        .email-header span {
            color: var(--secondary-color);
            font-size: 0.9em;
        }

        .email-body {
            font-size: 0.95em;
        }

        .strategy-notes {
            background-color: var(--note-bg);
            border: 1px solid #ffeeba;
            border-radius: 8px;
            padding: 20px;
        }

        .strategy-notes h3 {
            color: #856404;
            margin-bottom: 10px;
        }

        .strategy-notes ul {
            padding-left: 20px;
        }

        h2 {
            text-align: center;
            margin-bottom: 25px;
            color: var(--primary-color);
        }

        .navigation-buttons {
            display: flex;
            justify-content: space-between;
            padding: 20px 30px;
            border-top: 1px solid var(--border-color);
        }

        .nav-btn {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1em;
            transition: background-color 0.3s;
        }

        .nav-btn:hover {
            background-color: #0056b3;
        }
        
        .nav-btn:disabled {
            background-color: #c0c0c0;
            cursor: not-allowed;
        }
        
        .cta-button {
            background-color: var(--cta-color); 
            color: white; 
            padding: 15px 25px; 
            text-align: center; 
            text-decoration: none; 
            display: inline-block; 
            font-size: 16px; 
            border-radius: 8px;
            font-weight: bold;
            border: none;
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Proposta de Sequência de E-mails</h1>
            <p>"A Jornada de Leo" - Uma Novelinha para Nutrição de Leads</p>
        </header>

        <div class="nav-bar">
            <button class="nav-tab" data-slide="0">Intro</button>
            <button class="nav-tab" data-slide="1">E-mail 1</button>
            <button class="nav-tab" data-slide="2">E-mail 2</button>
            <button class="nav-tab" data-slide="3">E-mail 3</button>
            <button class="nav-tab" data-slide="4">E-mail 4</button>
            <button class="nav-tab" data-slide="5">E-mail 5</button>
        </div>

        <!-- Slide 0: Introdução -->
        <div class="slide">
            <h2>Bem-vindo(a) à Apresentação</h2>
            <div class="strategy-notes" style="background-color: #e2f0ff; border-color: #b8daff;">
                <h3 style="color:#004085;">Visão Geral da Estratégia</h3>
                <p>Esta sequência de 5 e-mails foi desenhada para nutrir os pais que baixaram o e-book "Os 100 primeiros dias", um público que está em um momento de alta vulnerabilidade e busca por direção.</p>
                <p><strong>A abordagem:</strong></p>
                <ul>
                    <li><strong>Hook, Story, Offer:</strong> Cada e-mail usa a metodologia de Gancho (assunto), História (o capítulo da "novelinha") e Oferta (um CTA sutil que evolui a cada passo).</li>
                    <li><strong>Novelinha Contínua:</strong> Criamos a família fictícia de "Ana, Marcos e Leo" para gerar uma conexão emocional forte e fazer o lead se sentir compreendido.</li>
                    <li><strong>Jornada de Confiança:</strong> O objetivo não é vender, mas sim construir uma relação de confiança tão sólida que agendar uma "Sessão de Acolhimento" se torne o próximo passo lógico e natural para a família.</li>
                </ul>
                <p>Clique em "Próximo" para ver o primeiro e-mail.</p>
            </div>
        </div>

        <!-- Slide 1: Email 1 -->
        <div class="slide">
            <h2>E-mail 1: O Silêncio no Carro</h2>
            <div class="slide-content">
                <div class="email-preview">
                    <div class="email-header">
                        <p><span>De:</span> Daiton Martins | CEDIN</p>
                        <p><strong>Assunto: O silêncio no carro, na volta para casa...</strong></p>
                    </div>
                    <div class="email-body">
                        <p>Olá, [Nome do Lead],</p>
                        <p>Sou Daiton Martins. Hoje, não quero falar como diretor de uma clínica, mas como alguém que já esteve sentado em frente a centenas de pais e mães como a Ana e o Marcos.</p>
                        <p><strong>(História - Capítulo 1)</strong><br>
                        Eu me lembro perfeitamente do dia em que os conheci. Eles me contaram sobre a volta para casa após receberem o laudo do filho, o Leo. O médico falou por uma hora, entregou uma pilha de papéis, mas a única coisa que ecoava na cabeça deles era uma palavra: <strong>autismo</strong>.</p>
                        <p>O caminho de volta foi em um silêncio profundo. Ana olhava pela janela, sentindo o peso do mundo. Marcos segurava o volante com força, tentando ser forte, mas sentindo o chão desaparecer. Em casa, o pequeno Leo brincava com seus carrinhos, alheio à tempestade que se formava ao seu redor.</p>
                        <p>Naquela noite, eles se sentiram completamente sozinhos. A mesma sensação que talvez você esteja sentindo agora.</p>
                        <p>Se essa história ressoa em você, quero que saiba de uma coisa que eu disse a eles naquele dia: "Isso que vocês sentem é o luto de um futuro que vocês imaginaram. Mas eu prometo, é também o exato ponto de partida para a construção de um novo futuro. Um futuro diferente, mas cheio de amor, descobertas e muitas alegrias."</p>
                        <p>Este é apenas o primeiro capítulo.</p>
                        <p>Com carinho,</p>
                        <p>Daiton Martins</p>
                        <hr><p><strong>P.S.:</strong> O guia que você baixou foi pensado exatamente para momentos como o da Ana e do Marcos. Se ainda não viu, a seção sobre "Acolhendo suas próprias emoções" pode ser um bom começo.</p>
                    </div>
                </div>
                <div class="strategy-notes">
                    <h3>Notas Estratégicas - E-mail 1</h3>
                    <ul>
                        <li><strong>Gancho:</strong> O assunto é emocional e misterioso, gerando curiosidade.</li>
                        <li><strong>Objetivo:</strong> Validação e Empatia. O foco é conectar-se com o sentimento de choque e solidão pós-diagnóstico.</li>
                        <li><strong>História:</strong> Apresenta os personagens e o conflito inicial, criando um espelho para a dor do lead.</li>
                        <li><strong>Oferta (CTA):</strong> Sutil e de baixo compromisso. Apenas relembra o valor do material que ele já possui, reforçando a autoridade.</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <!-- Slide 2: Email 2 -->
        <div class="slide">
            <h2>E-mail 2: O Labirinto de Siglas</h2>
            <div class="slide-content">
                <div class="email-preview">
                    <div class="email-header">
                        <p><span>De:</span> Daiton Martins | CEDIN</p>
                        <p><strong>Assunto: ABA, Denver, TEACCH... e o medo de escolher o caminho errado.</strong></p>
                    </div>
                    <div class="email-body">
                        <p>Olá, [Nome do Lead], tudo bem?</p>
                        <p>Continuando a história da família do Leo, quero te contar sobre a semana seguinte ao diagnóstico.</p>
                        <p><strong>(História - Capítulo 2)</strong><br>
                        O silêncio do carro deu lugar a um ruído ensurdecedor: o da internet. Ana passava as madrugadas no Google, mergulhando em um labirinto de siglas: ABA, Denver, TEACCH, PECS. Cada site prometia uma solução milagrosa, cada conselho parecia conflitante.</p>
                        <p>Marcos, por outro lado, tentava se afastar. Para ele, parecia que estavam tentando "consertar" o filho que ele amava. A tensão entre eles cresceu. O medo de Ana de "não fazer o suficiente" batia de frente com o medo de Marcos de "fazer a coisa errada".</p>
                        <p>Eles estavam em uma encruzilhada, paralisados pela quantidade de informação e pelo peso da responsabilidade. Foi quando eles entenderam que não precisavam de mais <em>informação</em>, mas sim de <em>direção</em>. Precisavam de alguém que traduzisse a ciência em um plano prático.</p>
                        <p>A busca deles não era mais por um método, mas por um parceiro.</p>
                        <p>Com carinho,</p>
                        <p>Daiton Martins</p>
                        <hr><p><strong>P.S.:</strong> Uma das siglas que mais confundia a Ana era ABA. Muitos a pintam como algo robótico, mas quando aplicada com amor, ela se torna uma ferramenta poderosa. Escrevi um artigo simples sobre isso, talvez ajude. [Link para o artigo do blog]</p>
                    </div>
                </div>
                <div class="strategy-notes">
                    <h3>Notas Estratégicas - E-mail 2</h3>
                    <ul>
                        <li><strong>Gancho:</strong> Toca em uma dor real: a confusão com os jargões técnicos.</li>
                        <li><strong>Objetivo:</strong> Educação e Posicionamento. Mostra que entendemos a sobrecarga de informação e começamos a posicionar o CEDIN como a "direção" necessária.</li>
                        <li><strong>História:</strong> Desenvolve o conflito, mostrando a paralisia causada pelo excesso de opções. Muitos pais se identificarão.</li>
                        <li><strong>Oferta (CTA):</strong> Educacional. Oferece mais valor (um artigo de blog), posicionando o CEDIN como um especialista que simplifica o complexo.</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Slide 3: Email 3 -->
        <div class="slide">
            <h2>E-mail 3: A Linguagem dos Carrinhos</h2>
            <div class="slide-content">
                <div class="email-preview">
                    <div class="email-header">
                        <p><span>De:</span> Daiton Martins | CEDIN</p>
                        <p><strong>Assunto: E então, no meio do caos, Leo nos mostrou o caminho.</strong></p>
                    </div>
                    <div class="email-body">
                        <p>Olá, [Nome do Lead],</p>
                        <p>O ponto de virada na jornada da Ana e do Marcos não veio de um livro ou de um especialista. Veio do próprio Leo.</p>
                        <p><strong>(História - Capítulo 3)</strong><br>
                        Numa tarde, eles encontraram o Leo no chão da sala. Ele tinha enfileirado seus carrinhos coloridos. Mas não era uma fila qualquer. Ele apontou para a fila e olhou para os dois, com uma intensidade que eles nunca tinham visto.</p>
                        <p>Naquele instante, Ana e Marcos entenderam. Aquela era a linguagem do Leo. Ele não estava "apenas enfileirando coisas". Ele estava se comunicando.</p>
                        <p>A epifania foi transformadora. Eles pararam de se perguntar "Como podemos fazer o Leo falar a nossa língua?" e começaram a se perguntar "<strong>Como podemos aprender a falar a língua do Leo?</strong>".</p>
                        <p>Essa mudança de perspectiva é a essência do que fazemos no CEDIN. Não se trata de encaixar a criança em um método, mas de construir uma ponte até o mundo dela.</p>
                        <p>Com carinho,</p>
                        <p>Daiton Martins</p>
                        <hr><p><strong>P.S.:</strong> A história do Leo é única, mas a transformação de sua família não é. Histórias de pais que aprenderam a "falar a língua" de seus filhos são o que nos move. Você pode ver algumas delas aqui. [Link para a página de depoimentos]</p>
                    </div>
                </div>
                <div class="strategy-notes">
                    <h3>Notas Estratégicas - E-mail 3</h3>
                    <ul>
                        <li><strong>Gancho:</strong> Evoca esperança e curiosidade. A solução vem da própria criança.</li>
                        <li><strong>Objetivo:</strong> Apresentar a filosofia do CEDIN e gerar esperança.</li>
                        <li><strong>História:</strong> É o clímax emocional. Mostra a "epifania" que muda a perspectiva dos pais do medo para a curiosidade e conexão. Conecta-se diretamente à filosofia do CEDIN.</li>
                        <li><strong>Oferta (CTA):</strong> Prova Social. Leva o lead para depoimentos, provando que essa transformação é real para outras famílias.</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Slide 4: Email 4 -->
        <div class="slide">
            <h2>E-mail 4: A Primeira Conversa</h2>
            <div class="slide-content">
                <div class="email-preview">
                    <div class="email-header">
                        <p><span>De:</span> Daiton Martins | CEDIN</p>
                        <p><strong>Assunto: O passo mais difícil: pedir ajuda.</strong></p>
                    </div>
                    <div class="email-body">
                        <p>Olá, [Nome do Lead],</p>
                        <p>Depois daquele dia dos carrinhos, Ana e Marcos sabiam o que procurar. Não uma clínica, mas um lugar que os ensinasse a construir pontes.</p>
                        <p><strong>(História - Capítulo 4)</strong><br>
                        Foi a Ana quem encontrou nosso site. Ela me confessou que o dedo dela tremeu sobre o botão de "agendar uma conversa". O medo de ser julgada, de ouvir mais termos técnicos, era enorme. Mas a imagem do Leo e seus carrinhos deu-lhe a coragem.</p>
                        <p>Eles agendaram o que chamamos de <strong>Sessão de Acolhimento</strong>. E foi exatamente isso: acolhimento. Eles não foram recebidos com uma prancheta, mas com um café e ouvidos atentos. Falaram por mais de uma hora sobre os medos, as alegrias e a fila de carrinhos.</p>
                        <p>Pela primeira vez, eles não se sentiram como pais de "uma criança com autismo". Sentiram-se como Ana e Marcos, pais do Leo. E viram na nossa frente não apenas terapeutas, mas parceiros.</p>
                        <p>Sair daquela sala foi com esperança, com um plano e, o mais importante, com a certeza de que não estavam mais sozinhos.</p>
                        <p>Com carinho,</p>
                        <p>Daiton Martins</p>
                        <hr><p><strong>P.S.:</strong> Aquela primeira conversa mudou tudo para a família do Leo. Se você sente que é o momento de dar esse passo, de ser ouvido e encontrar um parceiro, estamos aqui para você. [>> Clique aqui para saber como funciona a nossa Sessão de Acolhimento <<]</p>
                    </div>
                </div>
                <div class="strategy-notes">
                    <h3>Notas Estratégicas - E-mail 4</h3>
                    <ul>
                        <li><strong>Gancho:</strong> Toca na vulnerabilidade de admitir que precisa de ajuda.</li>
                        <li><strong>Objetivo:</strong> Apresentar a "solução" (Sessão de Acolhimento) e diminuir a barreira para o primeiro contato.</li>
                        <li><strong>História:</strong> Descreve a experiência de pedir ajuda não como algo clínico e frio, mas como um ato de acolhimento e parceria, quebrando as objeções do lead.</li>
                        <li><strong>Oferta (CTA):</strong> Direcionada. O CTA agora leva para uma página explicando a oferta principal (a sessão), preparando o terreno para a conversão final.</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Slide 5: Email 5 -->
        <div class="slide">
            <h2>E-mail 5: O Novo Começo</h2>
            <div class="slide-content">
                <div class="email-preview">
                    <div class="email-header">
                        <p><span>De:</span> Daiton Martins | CEDIN</p>
                        <p><strong>Assunto: A "novelinha" da Ana e do Marcos chegou ao fim... para que a sua possa começar.</strong></p>
                    </div>
                    <div class="email-body">
                        <p>Olá, [Nome do Lead],</p>
                        <p>Hoje, a história da família do Leo não é mais sobre o medo do diagnóstico. É sobre a alegria de ouvir a primeira frase completa, as vitórias de conseguir acalmar uma crise e a confiança de vê-lo interagir na escola.</p>
                        <p><strong>(História - Conclusão)</strong><br>
                        A jornada deles não é um conto de fadas. Tem dias difíceis. Mas agora eles têm ferramentas, apoio e a certeza de que não estão sozinhos.</p>
                        <p>Eu te contei essa "novelinha" por um motivo: para te mostrar que o caminho que parece tão escuro e solitário agora, pode se iluminar. Existe um futuro de conquistas para sua família.</p>
                        <p>A história de Ana, Marcos e Leo é uma inspiração. Agora, eu gostaria de ajudar a escrever a sua.</p>
                        <p><strong>(Oferta)</strong><br>
                        O primeiro capítulo da sua nova história pode começar com uma simples conversa. Um momento para você, sem compromisso, para ser acolhido(a) e encontrar a direção que precisa.</p>
                        <p>Convido você pessoalmente para a nossa <strong>Sessão de Acolhimento Gratuita</strong>. Deixe-nos ouvir sua história e mostrar como podemos caminhar juntos.</p>
                        <p>Com carinho,</p>
                        <p>Daiton Martins</p>
                        <br>
                        <button class="cta-button">Sim, quero começar a escrever minha história de conquistas</button>
                        <br><br>
                        <hr><p><strong>P.S.:</strong> Assim como demos atenção total à família do Leo, dedicamos nosso tempo a cada nova família. Por isso, as vagas para a Sessão de Acolhimento são limitadas. Garanta a sua clicando no botão acima.</p>
                    </div>
                </div>
                <div class="strategy-notes">
                    <h3>Notas Estratégicas - E-mail 5</h3>
                    <ul>
                        <li><strong>Gancho:</strong> Meta-linguagem que quebra a quarta parede e fala diretamente com o lead.</li>
                        <li><strong>Objetivo:</strong> Conversão. Levar o lead a agendar a Sessão de Acolhimento.</li>
                        <li><strong>História:</strong> Conclui a jornada da família fictícia, pintando um quadro de esperança e progresso. Transfere o foco da história deles para a história do lead.</li>
                        <li><strong>Oferta (CTA):</strong> Direta e clara. Um botão de CTA forte e um P.S. que adiciona um toque de escassez positiva para incentivar a ação.</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="navigation-buttons">
            <button class="nav-btn" id="prevBtn" disabled>Anterior</button>
            <button class="nav-btn" id="nextBtn">Próximo</button>
        </div>

    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const slides = document.querySelectorAll('.slide');
            const prevBtn = document.getElementById('prevBtn');
            const nextBtn = document.getElementById('nextBtn');
            const navTabs = document.querySelectorAll('.nav-tab');

            let currentSlide = 0;
            const totalSlides = slides.length;

            function showSlide(index) {
                slides.forEach((slide, i) => {
                    slide.style.display = i === index ? 'block' : 'none';
                });
                navTabs.forEach((tab, i) => {
                    tab.classList.toggle('active', i === index);
                });
                
                prevBtn.disabled = index === 0;
                nextBtn.disabled = index === totalSlides - 1;
                currentSlide = index;
            }

            nextBtn.addEventListener('click', () => {
                if (currentSlide < totalSlides - 1) {
                    showSlide(currentSlide + 1);
                }
            });

            prevBtn.addEventListener('click', () => {
                if (currentSlide > 0) {
                    showSlide(currentSlide - 1);
                }
            });

            navTabs.forEach(tab => {
                tab.addEventListener('click', () => {
                    const slideIndex = parseInt(tab.dataset.slide);
                    showSlide(slideIndex);
                });
            });

            // Show the first slide initially
            showSlide(0);
        });
    </script>

</body>
</html>

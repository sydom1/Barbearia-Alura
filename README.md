# Barbearia-Alura
Site responsivo da barbearia alura.
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barbearia Alura</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&family=Titillium+Web&display=swap" rel="stylesheet">
</head>

<body>
    <!-- estrutura do cabecalho-->
    <header>
        <div class="caixa">
            <h1><img src="logo.png" alt="Logo"></h1>

            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="Produtos.html">Produtos</a></li>
                    <li><a href="contato.html">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <img class="banner" src="banner.jpg">

    <main>
        <!--a section e usada no lugar da div, para agrupar o conteudo que tem 
        o mesmo sentido-->
        <section class="principal">
            <h2 class="titulo-principal">Sobre a Barbearia Alura</h2>

            <img class="utensilios" src="utensilios.jpg" alt="utensilios de barbeiro">

            <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o que há de melhor para o seu cabelo e barba. Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

            <p id="missao"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de vida aos clientes"</strong>.</em></p>

            <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. O atendimento possui padrão de excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
        </section>

        <section class="mapa">

            <h3 class="titulo-principal">Nosso estabelecimento</h3>
            <p>Nosso estabelecimento está localizado no coração da cidade</p>

            <div class="mapa-conteudo">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d234054.8195967066!2d-46.91538867500006!3d-23.5646162!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce59541c6c79c3%3A0x36b90a85f0f8cb33!2sGrupo%20Alura!5e0!3m2!1spt-PT!2sbr!4v1674608780338!5m2!1spt-PT!2sbr"
                    width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </section>

        <section class="beneficios">
            <h3 class="titulo-principal">Benefícios</h3>

            <div class="conteudo-beneficios">
                <ul class="lista-beneficios">
                    <li class="itens">Atendimento aos Clientes</li>
                    <li class="itens">Espaço diferenciado</li>
                    <li class="itens">Localização</li>
                    <li class="itens">Profissionais Qualificados</li>
                    <li class="itens">Pontualidade</li>
                    <li class="itens">Limpeza</li>
                </ul><img src="beneficios.jpg" class="imagem-beneficios">
            </div>

            <div class="video">
                <iframe width="100%" height="315" src="https://www.youtube.com/embed/wcVVXUV0YUY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
            </div>

        </section>
    </main>

    <footer>
        <img src="logo-branco.png" alt="logo">
        <p class="copyright">&copy; Copyright Barbearia Alura - 2019</p>
    </footer>
</body>

</html>


body {
    font-family: 'Montserrat', sans-serif;
}

header {
    background: #BBBBBB;
    /*cor de fundo cinza apenas no headr*/
    padding: 20px 0;
    /*para deixar o espaçamento do menu e imagem perfeitos p o site*/
}

.caixa {
    width: 940px;
    /*margem padrão web*/
    position: relative;
    /*foi usado para trazer o navegardo para a margem do width da caixa*/
    margin: 0 auto;
    /*para cima e baixo zero de margem, e o auto serve para o calculo ser feito automatico da direita e esqueda, centraliza automatico*/
}

nav {
    position: absolute;
    /*a posição absoluta server para deixar a objeto solto sempre usar para posicionar algo*/
    top: 110px;
    right: 0;
}

nav li {
    display: inline;
    /*colocar os intens em linha*/
    margin: 0 0 0 15px;
    /*colocar um espaçamento entre os itens a esqueda*/
}

nav a {
    text-transform: uppercase;
    /*colcar o texto em Maiusco*/
    color: #000000;
    /*cor do texto*/
    font-weight: bold;
    /*fonte negrito*/
    font-size: 22px;
    /*tamanho da fonte*/
    text-decoration: none;
    /*tira toda formatação do texto*/
}

nav a:hover {
    /*hover e pra adicionar comportamento quando o mouse estiver em cima do item*/
    color: #C78C19;
    text-decoration: underline;
}

.produtos {
    width: 940px;
    /*margem padrão web*/
    margin: 0 auto;
    /*para cima e baixo zero de margem, e o auto serve para o calculo ser feito automatico da direita e esqueda, centraliza automatico*/
    padding: 50px 0;
    /*aumentado a distancia para cima e para baixo*/
}

.produtos li {
    display: inline-block;
    /*colocando os itens ao lado um do outro*/
    text-align: center;
    /*centralizar os itens*/
    width: 30%;
    /*para deixar os itens com 30% de espaço kda*/
    vertical-align: top;
    /*alinhar pela parte de cima, ficar todos na mesma linha mais alinhando pelo item superior*/
    margin: 0 1.5%;
    /*espaçamento lateral, espaçamento externo*/
    padding: 30px 20px;
    /*espaçamento interno*/
    box-sizing: border-box;
    /*para não deixar que os espaçamentos se somem, que o intem trabalhe com o espaçamento definido*/
    border: 2px solid #000000;
    border-radius: 10px;
}

.produtos li:hover {
    /*hover e pra adicionar comportamento quando o mouse estiver em cima do item*/
    border-color: #C78C19;
}

.produtos li:active {
    /*adicionando quando o o item for clicado*/
    border-color: #088c19;
}

.produtos li:hover h2 {
    /*para mudar o elemento h2*/
    font-size: 34px;
}

.produtos h2 {
    font-size: 30px;
    /*tamanho da fonte*/
    font-weight: bold;
    /*peso da fonte negrito*/
}

.produto-descricao {
    font-size: 18px;
}

.produto-preco {
    font-size: 22px;
    /*tamanho da fonte*/
    font-weight: bold;
    /*peso da fonte negrito*/
    margin-top: 10px;
}

footer {
    text-align: center;
    background: url(bg.jpg);
    padding: 40px 0;
}

.copyright {
    color: #FFFFFF;
    font-size: 13px;
    margin-top: 20px 0 0;
}


/*pagina de contato*/


/*
main {
    width: 940px;
    margin: 0 auto;
}
*/

form {
    margin: 40px 0;
    padding-left: 5em;
}

form label,
form legend {
    display: block;
    font-size: 20px;
    margin: 0 0 10px;
}

.input-padrao {
    display: block;
    margin: 0 0 20px;
    padding: 10px 25px;
    width: 50%;
}

.checkbox {
    margin: 20px 0;
}


/*Botão enviar*/

.enviar {
    width: 40%;
    padding: 15px 0;
    background: orange;
    color: white;
    font-weight: bold;
    font-size: 18px;
    border: none;
    border-radius: 5px;
    transition: 1s all;
    /*sempre informar o que sera utilizado na transição, all são todos as
     configurações se usar o background so iria mudar o fundo*/
    /*para fazer a transição*/
    cursor: pointer;
    /*o tipo do cursor*/
}

.enviar:hover {
    background: rgb(255, 94, 0);
    /*para fazer a transição*/
    transform: scale(1.2);
    /*para aumentar o tamanho do botão*/
    /* transform: rotate(20deg); da o efeito de rotação, para colocar
     mais um transform e socolocar em ordem transform: rotate(20deg), scale(1.2);*/
}


/*tabela*/

table {
    margin: 20px 5em 40px;
}

thead {
    background: #555555;
    color: white;
    font-weight: bold;
}

td,
th {
    border: 1px solid #000000;
    padding: 8px 15px;
}


/*estilização da home-page*/

.banner {
    width: 100%;
}

.titulo-principal {
    text-align: center;
    font-size: 2em;
    /*o tipo "em" e utilizado quando querendo deixar o tamanho proporcionalo ao pixel
    nesse caso 2em significa que a fonte tera o dobro do tamnho do pixel das outras fontes*/
    margin: 0 0 1em;
    clear: left;
    /*pra colocar a imagem antes do texto de forma alinhada usado junto com o float dos
    utensilios*/
}

.titulo-principal::first-letter {
    font-weight: bold;
    /*pra deixar a primeira letra em negrito*/
}

.principal {
    padding: 3em 0;
    background: #FFFFFF;
    width: 940px;
    margin: 0 auto;
}

.principal p {
    margin: 0 0 1em;
}

.principal strong {
    font-weight: bold;
}

.principal em {
    font-style: italic;
}

.utensilios {
    width: 120px;
    float: left;
    /*pra colocar a imagem antes do texto de forma alinhada*/
    margin: 0 20px 20px 0;
}

.beneficios {
    padding: 3em 0;
    background: #888888;
}

.conteudo-beneficios {
    width: 640px;
    margin: 0 auto;
}

.lista-beneficios {
    width: 40%;
    display: inline-block;
    vertical-align: top;
}

.itens {
    line-height: 1.5;
}


/*
.itens::after {
    content: "🟊";
    coloca a estralinha nesse caso depois da palavra
}
*/

.itens::before {
    content: "🟊";
    /*coloca a estralinha nesse caso antes da palavra*/
}

.itens:first-child {
    font-weight: bold;
}


/*para alterar apenas o primeiro item da lista*/


/*caso fosse marcar outro item usariamos o nth-chid(aqui colocaria o ele mento
2n para todos os pares, ou 2 para segundo elemento) e last para o ultimo*/

.imagem-beneficios {
    width: 60%;
}

.mapa {
    padding: 3em 0;
    background: linear-gradient(#ffffff, #888888);
    /*fazer o degrade, aqui e o meio, podemos fazer a inclinação 
    usando deg (45deg) e se quiser dezier o quanto cada cor
    vai utilizar de espaço e so colocar a porcentagem 
    antes da cor tipo (50% red), se quiser o gradiente cricular e so usar
    o radial-gradient*/
}

.mapa-conteudo {
    width: 940px;
    margin: 0 auto;
}

.mapa p {
    margin: 0 0 2em;
    text-align: center;
}

.video {
    width: 560px;
    margin: 2em auto;
    opacity: 0.5;
    /*Opacidade para elemento*/
    transition: 400ms;
    box-shadow: 10px 15px 5px black;
    /*sombra, eixo Y, eixo X, intensidade da Borda e cor*/
}

.video:hover {
    opacity: 1;
    /*Opacidade para elemento*/
}


/*adaptação para dispositivos moveis*/

@media screen and (max-width: 480px) {
    .caixa,
    .principal,
    .conteudo-beneficios,
    .mapa-conteudo,
    .video {
        width: auto;
    }
    h1 {
        text-align: center;
    }
    nav {
        position: static;
    }
    .lista-beneficios,
    .imagem-beneficios {
        width: 100%;
    }
}

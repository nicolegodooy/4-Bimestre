# 4-Bimestre
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flashcards — Ditadura Militar no Brasil</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <main class="container">
        <header class="cabecalho">
            <span class="tag-materia">História do Brasil • 1964–1985</span>
            <h1>Flashcards: Ditadura Militar</h1>
            <p class="subtitulo">Clique no cartão para revelar a resposta</p>
        </header>

        <!-- Barra de Progresso -->
        <div class="progresso-wrapper">
            <span id="contadorCard" class="contador">Cartão 1 de 6</span>
            <div class="barra-fundo">
                <div id="barraProgresso" class="barra-preenchimento"></div>
            </div>
        </div>

        <!-- Área do Flashcard 3D -->
        <section class="cena-card">
            <div id="flashcard" class="flashcard" onclick="virarCard()" tabindex="0" role="button" aria-label="Virar cartão">
                
                <!-- Frente (Pergunta) -->
                <div class="face frente">
                    <span class="etiqueta">PERGUNTA</span>
                    <p id="textoPergunta" class="texto-card"></p>
                    <span class="dica-virar">↻ Toque para ver a resposta</span>
                </div>

                <!-- Verso (Resposta) -->
                <div class="face verso">
                    <span class="etiqueta">RESPOSTA</span>
                    <p id="textoResposta" class="texto-card"></p>
                    <span class="dica-virar">↺ Toque para voltar à pergunta</span>
                </div>

            </div>
        </section>

        <!-- Controles de Navegação e Acessibilidade -->
        <div class="controles">
            <button id="btnAnterior" class="btn-nav" onclick="mudarCard(-1)" title="Cartão anterior">
                ← Anterior
            </button>

            <button id="btnVoz" class="btn-voz" onclick="ouvirCard()" title="Ouvir texto do cartão">
                🔊 Ouvir
            </button>

            <button id="btnProximo" class="btn-nav btn-principal" onclick="mudarCard(1)" title="Próximo cartão">
                Próximo →
            </button>
        </div>
    </main>

    <script src="script.js"></script>
</body>
</html>

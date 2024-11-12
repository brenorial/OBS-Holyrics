## Integração OBS - Holyrics

Explicação do código CSS

### Passos iniciais
1. Habilitar plugin Holyrics em Ferramentas - Plugin. 
2. Adicionar fonte modelo Navegador no OBS, inserindo em URL o IP HTML 2 do Plugin.
3. Largura e Altura sugeridas: 2000 x 600
4. Inserir código no campo CSS Personalizado

### .bible-header-custom
Define um cabeçalho personalizado com um layout em grid e estilo específico:

- `display: grid;`: Configura o elemento para usar layout de grid.
- `align-content: center;`: Centraliza o conteúdo no eixo vertical.
- `width: fit-content;`: Ajusta a largura ao conteúdo interno.
- `padding: 4px 20px;`: Adiciona espaço interno de 4px em cima e embaixo e 20px nos lados.
- `position: absolute;`: Posiciona o elemento de forma absoluta em relação ao seu contêiner.
- `top: 70px; left: 10px;`: Define a posição do elemento a 70px do topo e 10px da esquerda.
- `background-color: #000; color: #fff;`: Define o fundo preto e o texto branco.
- `font-size: 20px;`: Define o tamanho da fonte em 20px.
- `border-radius: 35px;`: Adiciona bordas arredondadas com raio de 35px.

### .music-slide
Aplica uma sombra ao texto:

- `text-shadow: 1px 1px 20px rgba(0, 0, 0, 0.5);`: Adiciona uma sombra com deslocamento de 1px nos eixos x e y, com um desfoque de 20px e cor preta semitransparente.

### desc
Estiliza o elemento `desc` (assumindo que é uma tag personalizada) com:

- `font-size: 35px;`: Define o tamanho da fonte em 35px.

### .bible_slide
Define uma seção com aparência de slide bíblico:

- `display: grid;`: Define o layout como grid.
- `padding: 30px;`: Adiciona um preenchimento interno de 30px em todos os lados.
- `height: 150px;`: Define a altura do elemento em 150px.
- `border-radius: 20px;`: Arredonda as bordas com 20px.
- `color: #000;`: Define o texto na cor preta.
- `background-color: #f2eddb;`: Define o fundo com uma cor bege claro.

### .bible_slide > span
Define a exibição dos elementos `span` dentro de `.bible_slide`:

- `display: none;`: Oculta todos os elementos `span` filhos de `.bible_slide`.

### @keyframes fade-in
Define uma animação de aparecimento gradual:

- `from { opacity: 0.0; } to { opacity: 1.0; }`: A animação começa com o elemento invisível (`opacity: 0.0`) e o torna visível (`opacity: 1.0`).

### @keyframes fade-out
Define uma animação de desaparecimento gradual:

- `from { opacity: 1.0; } to { opacity: 0.0; }`: A animação começa com o elemento visível (`opacity: 1.0`) e o torna invisível (`opacity: 0.0`).

### desc, ctt, .music_slide
Aplica a animação de `fade-in` a esses elementos:

- `animation-name: fade-in;`: Nome da animação aplicada.
- `animation-duration: 0.5s;`: Define a duração da animação como 0,5 segundos.
- `animation-fill-mode: forwards;`: Mantém o estado final da animação após o término (elemento permanece visível).

Essa aplicação é um player de música simples que reproduz uma lista de músicas em sequência. Ele utiliza recursos do DOM para controlar os elementos HTML e do áudio para reproduzir as músicas.

## Funcionalidades
- Botão "Iniciar/Parar": Quando clicado, reproduz ou pausa a música atual.
- Botão "Próxima música": Avança para a próxima música da lista.
- Botão "Música anterior": Volta para a música anterior da lista.
- Ícone de coração: Permite favoritar a música atual. Ao clicar no ícone, a cor muda para vermelho se a música estiver favoritada, e volta para branco se não estiver favoritada.
- Barra de volume: Permite ajustar o volume do áudio.
- Tecla "M": Alterna entre volume 0 e o volume anteriormente selecionado. Se o volume estiver em 0, o áudio é pausado.
- Tecla "K": Inicia ou para a reprodução da música atual.
- Teclas de seta (esquerda/direita): Avança ou retrocede para a próxima ou música anterior, respectivamente.

## Explicação
A primeira parte do código é responsável por selecionar os elementos HTML necessários para a interação com o usuário. Os elementos são selecionados usando o método querySelector, e as referências a eles são armazenadas em variáveis para uso posterior. Por exemplo, const iniciar = document.querySelector('.iniciar'); seleciona o elemento HTML com a classe "iniciar" e o armazena na variável iniciar.

Em seguida, temos a definição de um array chamado musicas que contém os detalhes das músicas que serão reproduzidas. Cada objeto no array representa uma música e possui propriedades como nomeMusica, nomeCantor, src (o caminho para o arquivo de áudio) e imagem (o caminho para a imagem da capa da música).

Existem várias variáveis declaradas que são usadas para controlar o estado da aplicação. Algumas delas são:

indiceMusicaAtual: Armazena o índice da música atualmente em reprodução no array musicas.
rotateIntervalId: Armazena o ID do intervalo utilizado para girar a imagem da capa da música.
tempoReproducao e tempoPausado: Armazenam o tempo atual de reprodução e pausa da música, respectivamente.
musicaAtual: Armazena o objeto da música atualmente em reprodução.
A função reproduzirMusica() é responsável por iniciar a reprodução da música. Ela é chamada quando o botão "Iniciar/Parar" é clicado. Essa função realiza várias tarefas, como interromper a música atualmente em reprodução (se houver), obter os detalhes da próxima música a ser reproduzida a partir do array musicas, atualizar os elementos HTML com os detalhes da música (nome, cantor, imagem), iniciar a rotação da imagem da capa, atualizar o progresso da música e reproduzir o áudio.

A função pararMusica() é responsável por interromper a reprodução da música atual. Ela é chamada quando o botão "Parar" é clicado ou quando uma nova música é selecionada. Essa função para a rotação da imagem, armazena o tempo de reprodução atual, pausa o áudio, remove o evento de atualização do progresso da música e atualiza a visibilidade dos botões HTML.

Outras funções, como verificarSeMusicaFavoritada() (para verificar e atualizar o status de favoritos da música atual) e atualizarProgresso() (para armazenar o tempo de pausa da música), são usadas para tarefas específicas.

Existem também os event listeners que respondem a diferentes eventos, como cliques em botões, alterações na barra de volume e pressionar teclas específicas. Esses event listeners chamam as funções correspondentes para executar a lógica apropriada.

No geral, o código controla a reprodução de músicas, a atualização dos elementos HTML, o controle do volume, a rotação da imagem da capa e a interação com o usuário. Ele utiliza recursos do DOM e do áudio para fornecer uma experiência básica de reprodução de músicas em sequência.

## Tecnologias / Tecnologies
- ``HTML``
- ``CSS``
- ``JavaScript``


<p>Feito com ❤️ por Leonardo Machado 👋🏽 [Entre em contato!](https://www.linkedin.com/in/leonardommachado/) </p>

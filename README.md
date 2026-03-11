# Flappy Bird — Trabalho Final Intro IA

Projeto do trabalho final da disciplina "Introdução à Inteligência Artificial": uma implementação em Python do jogo Flappy Bird.

**Descrição**

Uma versão simples do Flappy Bird desenvolvida em Python. Inclui o arquivo principal com o jogo (`FlappyBird.py`) e um arquivo com o gabarito/solução (`Gabarito FlappyBird.py`). Imagens e recursos gráficos ficam na pasta `imgs/`.

**Funcionalidades**

- Jogo jogável com controles simples (pular/voar)
- Pontuação e detecção de colisões
- Código organizado para estudo e modificação

**Requisitos**

- Python 3.8+ recomendado
- Biblioteca `pygame` (para execução do jogo)

**Instalação**

1. Crie e ative um ambiente virtual (opcional, recomendado):

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS / Linux
source venv/bin/activate
```

2. Instale o Pygame:

```bash
pip install pygame
```

**Como executar**

Para iniciar o jogo principal:

```bash
python "FlappyBird.py"
```

Para executar o arquivo gabarito/solução:

```bash
python "Gabarito FlappyBird.py"
```

**Controles**

- Pressione `Espaço` ou clique com o mouse para fazer o pássaro pular.

**Estrutura do projeto**

- [FlappyBird.py](FlappyBird.py) — arquivo principal do jogo
- [Gabarito FlappyBird.py](Gabarito FlappyBird.py) — exemplo/gabarito
- [config.txt](config.txt) — configurações auxiliares
- [informacoes.md](informacoes.md) — notas e informações do projeto
- [imgs](imgs) — recursos gráficos (sprites, fundos, etc.)

**Como contribuir**

Se quiser melhorar o jogo ou adaptar para estudos, abra uma issue ou envie um pull request com as modificações. Sugestões comuns:

- Ajustar física do pulo
- Adicionar novos níveis ou elementos
- Melhorar arte e áudio

**Autor**

- Trabalho desenvolvido por você como parte da disciplina.

**Licença**

Licença MIT — sinta-se à vontade para usar e modificar para fins educativos.

**Configuração NEAT (IA)**

O arquivo `config.txt` contém as configurações do algoritmo NEAT usado para treinar redes neurais que controlam os pássaros no modo IA. Essas configurações definem parâmetros como taxa de mutação, tamanho da população, parâmetros de crossover, limites de compatibilidade de espécies e critérios de estagnação. Durante a execução com IA (`Gabarito FlappyBird.py`), o NEAT roda por gerações — a cada geração a população é avaliada pela função `main`, os genomas recebem fitness e, ao longo das gerações, as redes tendem a melhorar seu desempenho.

Se quiser ajustar o treinamento (por exemplo, número de gerações ou parâmetros evolutivos), edite `config.txt` conforme a sintaxe do NEAT-Python.

**Qual arquivo usar**

- `Gabarito FlappyBird.py`: versão funcional com suporte a IA. Quando a variável `ai_jogando` está definida como `True`, o programa usa o NEAT para treinar e executar agentes controlados por redes neurais. Use este arquivo para treinar e avaliar modelos.
- `FlappyBird.py`: versão para jogo manual, destinada ao jogador humano. Execute este arquivo se quiser jogar sem ativar o sistema de IA.

**Dicas rápidas**

- Para treinar IA: garanta que `ai_jogando = True` em `Gabarito FlappyBird.py` e execute-o; o processo utilizará `config.txt`.
- Para jogar manualmente: abra `FlappyBird.py` e execute-o; use `Espaço` para pular.



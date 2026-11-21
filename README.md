# Filosofle

Jogo de palavras inspirado no Wordle, com conceitos de Filosofia, pistas progressivas após erros e explicações de significado, origem, exemplos e aprofundamento.

## Jogar

Abra `index.html` no navegador ou use o endereço do GitHub Pages após a publicação.

O jogo é feito com HTML, CSS e JavaScript. A versão publicada é um arquivo único, sem necessidade de instalar pacotes, criar conta ou configurar servidor. O progresso é armazenado localmente no navegador.

## Publicação

O arquivo `index.html` está na raiz da branch `main`. Para ativar o GitHub Pages, em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/(root)** e clique em **Save**.

Endereço esperado após ativação: https://henriqueocampospinarello-bot.github.io/Filosofle/

## Verificação das tentativas

O Wordle aceita apenas palavras reconhecidas por uma base lexical de português brasileiro, ou os conceitos de Filosofia que constam do próprio jogo. Uma tentativa não reconhecida **não gasta** uma chance.

A base externa é a lista [Palavras PT-BR](https://github.com/pythonprobr/palavras), derivada do dicionário ortográfico VERO/LibreOffice e disponibilizada sob a [licença MPL 2.0](https://github.com/pythonprobr/palavras/blob/master/LICENSE). O navegador consulta a lista pela internet e tenta armazená-la em cache para visitas seguintes. Trata-se de um vocabulário amplo, mas nenhuma lista fixa consegue conter todas as palavras, neologismos, regionalismos ou formas flexionadas do português.

O tamanho do dicionário não é apresentado na interface do jogo. Em caso de falha no carregamento, o site pede conexão para validar palavras que não estejam no banco dos próprios conceitos filosóficos.

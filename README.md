# Filosofle

Jogo de palavras inspirado no Wordle, com 138 conceitos selecionados de oito áreas da Filosofia, pistas progressivas após erros e explicações de significado, origem, exemplos e aprofundamento.

Veja a lista completa de respostas em [PALAVRAS.md](PALAVRAS.md). O banco de respostas é separado do dicionário geral de tentativas.

## Jogar

Abra `index.html` no navegador ou use o endereço do GitHub Pages após a publicação.

O jogo é feito com HTML, CSS e JavaScript. A versão publicada é um arquivo único, sem necessidade de instalar pacotes, criar conta ou configurar servidor. O progresso é armazenado localmente no navegador.

## Publicação

O arquivo `index.html` está na raiz da branch `main`. Para ativar o GitHub Pages, em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/(root)** e clique em **Save**.

Endereço esperado após ativação: https://henriqueocampospinarello-bot.github.io/Filosofle/

## Verificação das tentativas

O Wordle aceita apenas palavras reconhecidas por uma base lexical de português brasileiro, ou os conceitos de Filosofia que constam do próprio jogo. Uma tentativa não reconhecida **não gasta** uma chance.

A base principal é [Palavras PT-BR](https://github.com/pythonprobr/palavras), derivada do dicionário ortográfico VERO/LibreOffice (licença MPL 2.0). Como complementos, são consultados o [léxico e as conjugações verbais](https://github.com/fserb/pt-br) (licença MIT) para ampliar a aceitação de plurais e verbos flexionados. Alguns exemplos frequentes, como **ações**, **virtudes**, **pensando**, **agiu** e **reflete**, são incluídos diretamente. Trata-se de um vocabulário amplo, mas nenhuma lista fixa garante todas as variações legítimas do português.

O tamanho do dicionário não é apresentado na interface do jogo. Em caso de falha no carregamento, o site pede conexão para validar palavras que não estejam no banco dos próprios conceitos filosóficos.

# Filosofle

Jogo de palavras inspirado no Wordle, com 86 conceitos selecionados de seis áreas da Filosofia, pistas progressivas após erros e explicações de significado, origem, exemplos e aprofundamento.

Veja a lista completa de respostas em [PALAVRAS.md](PALAVRAS.md). O banco de respostas é separado do dicionário geral de tentativas.

## Jogar

Abra `index.html` no navegador ou use o endereço do GitHub Pages após a publicação.

O jogo oferece Jogo livre e Sem pistas, sem uma aba separada de desafios. As descobertas, vitórias e partidas são calculadas somente a partir das 86 palavras atuais, preservando a possibilidade de revisar as palavras ainda não acertadas na seção Derrotas. A migração do histórico acontece uma única vez.

O jogo é feito com HTML, CSS e JavaScript. A versão publicada é um arquivo único, sem necessidade de instalar pacotes, criar conta ou configurar servidor. O progresso é armazenado localmente no navegador.

## Publicação

O arquivo `index.html` está na raiz da branch `main`. Para ativar o GitHub Pages, em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/(root)** e clique em **Save**.

Endereço esperado após ativação: https://henriqueocampospinarello-bot.github.io/Filosofle/

## Verificação das tentativas

O Wordle aceita apenas palavras reconhecidas por uma base lexical de português brasileiro, ou os conceitos de Filosofia que constam do próprio jogo. Uma tentativa não reconhecida **não gasta** uma chance.

O jogo reúne **três fontes de vocabulário diferentes**, carregadas de forma independente (com espelhos de download e cache no navegador):

1. **[Palavras PT-BR (pythonprobr)](https://github.com/pythonprobr/palavras):** lista derivada do VERO/LibreOffice (MPL 2.0).
2. **[fserb/pt-br](https://github.com/fserb/pt-br):** léxico geral e arquivo adicional de conjugações verbais (MIT).
3. **[palavras-ptbr, de Gerson Locci](https://github.com/gelocci/palavras-ptbr):** lista por frequência de uso, baseada em corpora da Leipzig Corpora Collection. Licença CC BY 4.0; crédito a Gerson Locci e aos dados da Leipzig. Somente as entradas classificadas como `correto` entram na validação.

As listas são combinadas **somente para validar tentativas**, nunca para ampliar as 86 respostas filosóficas. O jogo também reconhece plurais regulares a partir de formas singulares já registradas (como *paradigmas*, *animais*, *homens*, *flores*) e inclui flexões comuns diretamente (*ações*, *pensando*, *agiu*, *assassino*, *assassina*). Uma tentativa ausente de todas as bases não consome chance; enquanto um dos dicionários ainda carrega, o jogo pede para repetir a tentativa. A cobertura é ampla, mas não garante todas as flexões, regionalismos ou neologismos.

O tamanho do dicionário não é apresentado na interface do jogo. Em caso de falha no carregamento, o site pede conexão para validar palavras que não estejam no banco dos próprios conceitos filosóficos.

## Explicações ampliadas

Os 86 conceitos têm origem histórica, autores, relações entre ideias e controvérsias editoriais distribuídas nos arquivos de `conteudos/`. A explicação de **arché** na entrada *Acidente* distingue a busca pré-socrática por princípios da metafísica aristotélica de substância e acidente.

## Flexões

O jogo já aceita os pares de gênero revisados, plurais regulares e formas irregulares da lista interna, além dos dicionários externos. Não é possível prometer cobertura de 99% do português sem uma avaliação lexical representativa.

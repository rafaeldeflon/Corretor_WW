# Corretor_WW

>EN

Spell checker in PT-BR with chemistry theme, made along with the course "Spell Checker in Python: applying NLP techniques" taught by Professor Guilherme Santos da Alura.

This document describes the steps performed on the notebook.

## Handling the corpus

### About *corpus*

For the construction of the corrector it is necessary to have a database formed by words that exist and are written in the correct way, the *corpus*. The construction of the corpus is crucial for the corrector's conclusion, it is necessary to be aware of the number of different words and the plurality of word themes, for example.

In this project, the corpus was built from the book "Quimica, COLEÇÃO TEMAS DE FORMAÇÃO, VOLUME 3" produced by UNESP, so that the word base was formed by terms common to chemistry learning, which are not so found in other sources, enabling the use of this corrector to help teaching chemistry, for example.

### Working with *corpus*

First, the book in PDF format is transformed into .txt format, so that it can be processed in the notebook.

Then it was imported into the work environment, where, with the tools of the NLTK library, the text words were tokenized, the repeated ones were excluded and other unwanted words (stopwords) were eliminated.

## Building the broker

The spell checker is built around 4 word correction functions: one to add missing letters, one to eliminate excess letters, one to change two letters in place and one to replace a misspelled letter. After generalizing all the options, it indicates the most recurrent word in the corpus.

## Evaluating the spell checker

To know the efficiency of the spell checker, which in this case would be the percentage of correctness of the code in indicating existing words that correct the wrong words, a list with 187 words was used containing different spelling errors, in which the spell checker should indicate a word to correct .

The spell checker was able to indicate 65% of the existing words in the corpus, which is not a very high efficiency in general terms, but taking into account that the corpus in question is quite thematized, the spell checker would have potential use in it's purpose.

>PT-BR

Corretor ortográfico em PT-BR com temática de química, feito junto ao curso "Corretor Ortográfico em Python: aplicando técnicas de NLP" ministrado pelo professor Guilherme santos da Alura.

Neste documento há a descrição dos passos realizados no notebook.

## Tratando o corpus

### Sobre o *corpus*

Para a construção do corretor é preciso haver uma base de dados formada por palavras que existam e estejam escritas da maneira correta, o *corpus*. A construção do corpus é crucial para conclusão do corretor, precisa-se estar atento a quantidade de palavras diferentes entre si e a pluralidade de temas de palavras, por exemplo.

Neste projeto o corpus foi construído a partir do livro "Quimica, COLEÇÃO TEMAS DE FORMAÇÃO, VOLUME 3" produzido pela UNESP, para que a base de palavras fosse formada por temos comuns ao aprendizado de química, que não são tão encontrados em outras fontes, possibilitando o uso deste corretor no auxilio do ensino de química, por exemplo.

### Trabalhando com o *corpus*

Primeiramente o livro em formato PDF for transformado em formato .txt, para que fosse tratado no notebook.

Em seguida ele foi importado no ambiente de trabalho, onde, com o ferramental da biblioteca NLTK, tolkenizou-se as palavras dos texto, excluiu-se as repetidas e eliminou-e outras palavras indesejadas (stopwords).

## Construindo o corretor

O corretor foi construído com base em 4 funções de correção de palavras: uma para acrescentar letras faltantes, uma para eliminar letras excedentes, uma para trocar duas letras de lugar e uma para trocar uma letra digitada errada. Após geral todas as opções ele indica a palavra mais recorrente no corpus.

## Avaliando o corretor

Para saber a eficiência do corretor, que no caso seria a porcentagem de acerto do código em indicar palavras existentes que corrijam as palavras erradas, foi utilizada um lista com 187 palavras contendo diferentes erros de grafia, no qual o corretor deveria indicar uma palavra para corrigir.

O corretor foi capaz de indicar 65% de palavras existentes no corpus, o que não é uma eficiência muito grande avaliando-se de maneira geral, mas levando-se em consideração que o corpus em questão é bastante tematizado, o corretor teria potencial uso em seu propósito.



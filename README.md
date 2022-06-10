# Corretor_WW

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

Para saber a eficiência do correto, que no caso seria a porcentagem de acerto do código em indicar palavras existentes que corrijam as palavras erradas, foi utilizada um lista com 187 palavras contendo diferentes erros de grafia, no qual o corretor deveria indicar uma palavra para corrigir.

O corretor foi capaz de indicar 65% de palavras existentes no corpus, o que não é uma eficiência muito grande avaliando-se de maneira geral, mas levando-se em consideração que o corpus em questão é bastante tematizado, o corretor teria potencial uso em seu propósito.



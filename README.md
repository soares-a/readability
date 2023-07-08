# Legibilidade

Programa para calcular o nível de leitura de diferentes textos

Este programa em C, chamado "readability", calcula o índice de legibilidade Coleman-Liau de um texto fornecido pelo usuário. O índice Coleman-Liau é usado para determinar o nível de leitura necessário para entender o texto. O programa conta o número de letras, palavras e frases no texto e usa essas informações para calcular o índice Coleman-Liau.

## Como usar o programa

Compile o programa: ```gcc -o readability readability.c -lcs50 -lm```

Execute o programa: ```./readability```

Será solicitado que você insira o texto para análise.
O programa calculará o índice Coleman-Liau com base no texto fornecido.
O programa exibirá o nível de leitura correspondente ao índice.

### Detalhes de implementação

O programa utiliza a biblioteca ```cs50.h``` para obter entrada do usuário e a biblioteca ```stdio.h``` para entrada/saída de dados. Além disso, são utilizadas as bibliotecas ```string.h```, ```ctype.h``` e ```math.h``` para realizar operações com strings, verificar caracteres alfabéticos e realizar cálculos matemáticos, respectivamente.

## O programa é dividido em várias funções:

```count_letters```: conta o número de letras no texto.

```count_words```: conta o número de palavras no texto.

```count_sentences```: conta o número de sentenças no texto.

```calculate_index```: calcula o índice Coleman-Liau com base no número de letras, palavras e sentenças.

```print_grade```: exibe o nível de leitura correspondente ao índice.

O programa solicita ao usuário que insira um texto e, em seguida, chama as funções para contar as letras, palavras e sentenças. Em seguida, o índice Coleman-Liau é calculado e o nível de leitura correspondente é exibido na saída.

O programa trata casos especiais em que o índice é menor que 1 ou igual ou maior que 16, exibindo "Before Grade 1" e "Grade 16+" respectivamente.

## Requisitos

Compilador C

Biblioteca CS50

## Compilação

### Para compilar o programa, siga as etapas abaixo:

Certifique-se de ter um compilador C instalado em seu sistema.
Baixe e instale a biblioteca CS50, se ainda não estiver instalada.
Abra um terminal e navegue até o diretório do projeto.
Compile o programa usando o comando gcc: ```gcc -o readability readability.c -lcs50```

## Execução
Após a compilação bem-sucedida, você pode executar o programa da seguinte maneira:


```./readability```

O programa solicitará que você insira um texto para análise. Digite o texto desejado e pressione Enter. Em seguida, o programa calculará o índice Coleman-Liau com base no texto fornecido e exibirá o nível de leitura correspondente.

## Exemplos de Uso
### Aqui estão alguns exemplos de como executar e usar o programa:

$ ```./readability```

Text: Parabéns! Hoje é o seu dia. Você está indo para Lugares Fantásticos! Você está indo embora!
`Nível de Leitura: 3`

$ ```./readability```
Text: Harry Potter era um menino muito incomum de várias maneiras. Em primeiro lugar, ele odiava as férias de verão mais do que qualquer outro período do ano. Além disso, ele realmente queria fazer sua lição de casa, mas era obrigado a fazê-la em segredo, no meio da noite. E ele também aconteceu de ser um bruxo.
`Nível de Leitura: 5`

$ ```./readability```
Text: À medida que o número médio de letras e palavras por frase aumenta, o índice Coleman-Liau atribui ao texto um nível de leitura mais alto. Se pegarmos este parágrafo, por exemplo, que tem palavras e frases mais longas do que qualquer um dos dois exemplos anteriores, a fórmula atribuiria ao texto um nível de leitura de graduação sênior.
`Nível de Leitura: 12`

## Notas
O programa considera letras como caracteres alfabéticos maiúsculos e minúsculos, excluindo pontuação, dígitos e outros símbolos.
Uma palavra é definida como uma sequência de caracteres separados por espaços.
Uma sentença é definida como qualquer sequência de caracteres terminada por um ponto, ponto de exclamação ou ponto de interrogação.
Divirta-se usando o programa para calcular o nível de leitura de diferentes textos!

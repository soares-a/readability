# Primeiro, são incluídas as bibliotecas necessárias:

#include `<cs50.h>`: Essa biblioteca fornece a função get_string, que é usada para obter a entrada do usuário.

#include `<stdio.h>`: Essa biblioteca fornece funções para entrada/saída, como printf.

#include `<string.h>`: Essa biblioteca fornece funções para manipulação de strings.

#include `<ctype.h>`: Essa biblioteca fornece funções para manipulação de caracteres.

#include `<math.h>`: Essa biblioteca fornece funções matemáticas, como round.

## Em seguida, são declarados os protótipos das funções que serão implementadas posteriormente.

A função `main` é definida. É a função principal que será executada quando o programa for iniciado.

Dentro da função `main`:

É solicitado ao usuário que insira um texto usando a função `get_string` e armazena-o na variável text.

São contadas as letras, palavras e sentenças no texto usando as funções `count_letters`, `count_words` e `count_sentences`, 
respectivamente. Os resultados são armazenados nas variáveis `letters, words e sentences`.

O índice de Coleman-Liau é calculado usando a função `calculate_index` e os valores de letters, words e sentences. 
O resultado é armazenado na variável index.

O nível de série é impresso na saída usando a função `print_grade` e o valor de `index`.

As funções `count_letters`, `count_words` e `count_sentences` são definidas:

`count_letters` percorre cada caractere do texto e verifica se é uma letra usando a função `isalpha`. 
Se for uma letra, o contador count é incrementado.

`count_words` percorre cada caractere do texto e verifica se é um espaço em branco usando a função `isspace`. 
Se for um espaço em branco, o contador count é incrementado. O número total de palavras é igual a count + 1.

`count_sentences` percorre cada caractere do texto e verifica se é um ponto final, ponto de exclamação ou ponto de interrogação. 
Se for um desses caracteres, o contador count é incrementado.

A função `calculate_index` é definida:

Ela calcula os valores de L (número médio de letras por 100 palavras) e S (número médio de sentenças por 100 palavras) usando os parâmetros letters, words e sentences.

O índice de Coleman-Liau é calculado usando a fórmula fornecida na especificação do problema e retorna o resultado.

A função `print_grade` é definida:

Ela recebe o índice de Coleman-Liau como parâmetro e imprime o nível de série correspondente. 

Se o índice for menor que 1, imprime `"Before Grade 1"`. Se o índice for maior ou igual a 16, imprime `"Grade 16+"`. 

Caso contrário, imprime `"Grade X"`, onde X é o valor do índice.

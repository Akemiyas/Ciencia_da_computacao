### A diferença do início dos programas
**Algoritmos [Cap. 2]:**
No pseudocódigo ou fluxograma, a lógica exige demarcar onde as coisas começam e terminam para não gerar loops infinitos. Demarcada pelas palavras INÍCIO e FIM ou pela figura oval no topo do fluxograma:
`*/Apesar de utilizamos textos em português ao digitar pseudocódigos, toda linguagem de programação formal, para ser aceita mundialmente como ferramenta de trabalho, é sempre definida em inglês.E, se escrito manualmente, nunca deve conter letras minúsculas, e o zero deve vir acompanhado de um traço perpendicular, semelhante ao símbolo de conjunto vazio./*`

**C [Cap.2]:**
O C é composto por funções, sendo a principal a `main()`, os parênteses após a palavra indicam que é um bloco de construção do programa, ou seja, uma função. Todos os programas em C começam a ser executados pela função main. O bloco é uma unidade importante e são mostrados através das chaves `{`, para começar o corpo e `}` para terminar.

**Python [Cap. 1]:**
As três primeiras linhas ao iniciar o interpretador do Python contém informações sobre o interpretador e o sistema operacional em que está sendo executado. Após conferir também o número da versão basta fazer um teste de soma, pressionar Enter e observar se o resultado é exibido. Dado os fatos, podemos dizer que para inicializar um programa em python basta o interpretador abrir o arquivo `.py` e começar a ler freneticamente da linha 1 para baixo, executando o que vê pela frente.

### Entrada e Saída de dados
Para o programa ser útil, ele precisa receber dados do usuário (Entrada) e devolver um resultado (Saída).

**Algoritmos [Cap. 2]:**
No pseudocódigo, usamos os comandos `LEIA()` para capturar e `ESCREVA()` para mostrar na tela. //A lista com os comandos em português estruturado estarão no final da página.

**C [Cap.2]:**
O C exige saber o tipo de dado que está entrando ou saindo. Usamos a biblioteca `<stdio.h>` porque o receber e devolver não faz parte da linguagem de programação C, mas são funções desta biblioteca.
*   **Saída (`printf`):** Imprime na tela. O `f` significa format.
    ```c
    printf("Bem-vindo ao C!\n");
    ```
    Imprime na tela a string de caracteres limitada pelas aspas. A linha inteira, completa, é chamada de instrução, e toda instrução deve terminar com um ponto e vírgula (`;`). O `\n`, apesar de estar entre as aspas, não é impresso pois é está com uma backlash, caractere de escape. Veja as sequências de escape no final da página.
*   **Entrada (`scanf`):** Lê do teclado. Exige o uso do `&` (e comercial) para apontar para o endereço físico da variável na memória RAM.

`/*Por não fazerem parte da linguagem, o compilador não pode encontrar um erro de digitação em printf e scanf, ele apenas abre espaço no programa objeto para uma “chamada” à função da biblioteca. O compilador não sabe onde as funções da biblioteca se encontram, mas o linker sabe, e ele que localizará o erro.*/`

**Python [Cap.2 e 5]:**
O Python simplifica o processo unindo a mensagem de tela e a captura de dados no mesmo comando, sem precisar do endereço de memória (`&`).
*   **Saída: `print()`**
    ```python
    >>> print('Hello, World!')
    Hello, World
    ```
    As aspas marcam o começo e o fim do texto a ser exibido, elas não aparecem no resultado. Os parênteses indicam que o print é uma função.
*   **Entrada: `input()`** //Encontrada no capítulo 5
    ```python
    idade = input("Digite sua idade: ") # Faz a saída da pergunta e a entrada do dado de uma vez
    ```

### Tipos de Dados e Variáveis [Algoritmos Cap. 3]
Os dados são elementos do mundo exterior que representam, dentro de um computador digital, as informações manipuladas pelos seres humanos. Eles podem ser classificados em três tipos primitivos ou tipos básicos: numéricos, caracteres, e lógicos.
Variável é tudo que está sujeito a variações, que é incerto, instável ou inconstante. É necessário saber o tipo de dado para depois fazer seu armazenamento adequado, e armazenado o dado desejado, ele pode ser utilizado e processado a qualquer momento. Como uma "gaveta" na Memória RAM com uma etiqueta (nome) e um formato específico, usada para guardar um dado.

O nome de uma variável é utilizado para sua identificação e representação em um programa de computador e deve seguir algumas regras:
*   Podem utilizar um ou mais caracteres, limitando-se a restrições da própria linguagem formal de programação em uso (no caso do português estruturado, essa restrição não existe).
*   O primeiro caractere de identificação do nome de uma var. não pode ser numérico ou símbolo gráfico, sempre deve ser alfabético (os demais caracteres podem ser alfanuméricos).
*   Não pode haver espaços em branco. Caso deseje, pode-se utilizar o caractere de separação `_` underline.
*   Jamais deve ser definida com o mesmo nome de uma palavra que represente um dos comandos ou instruções de uma linguagem de programação de computadores. (Veja a lista das palavras reservadas em C, Python e português estruturado nas páginas finais.)
*   Não pode ser algum rótulo que já tenha sido usado para identificar o nome de um programa ou mesmo de outra variável. Um nome torna-se exclusivo no programa em que foi definido. (Em C, temos escopos diferentes e as variáveis locais podem ter o mesmo nome em outro escopo, apenas variáveis globais ou locais, no local que foi definido, não podem ter nomes iguais).

A variável pode assumir um papel de ação, quando o valor inicial é modificado ao longo da execução de um programa, ou papel de controle, quando seu valor é “vigiado” e utilizado em operações lógicas de decisão e laços de repetição ao longo de um programa. Ou seja, uma variável é a representação de uma região de memória utilizada para armazenar, acessar e modificar certo valor por um determinado espaço de tempo.

`*/Uma boa prática é escolher nomes significativos para as variáveis, ajudando a tornar um programa auto-explicativo/*`
`*/O C faz distinção entre letras maiúsculas e minúsculas (case sensitive, sensível a caixa alta/baixa) e por isso a1 e A1 são identificadores diferentes. Identificadores que começam com uma letra maiúscula serão atribuídos a um significado especial, que será visto posteriormente. /*`

**Algoritmos [Cap.3]:**
*   **Inteiro:** Números pertencentes ao conjunto de números inteiros, sem casas decimais (ex: 10, -5). O tipo de dado inteiro é utilizado em operações de processamento matemático. Em português estruturado, a representação do dado inteiro é feita com o comando INTEIRO.
*   **Real:** Números pertencentes ao conjunto de números reais, com casas decimais, fracionários e inteiros (ex: 4.50, 3.14). Em português estruturado, representado pelo comando REAL. O tipo de dado real é utilizado em operações de processamento matemático.
*   **Caractere / Cadeia:** Textos ou letras soltas, delimitados por aspas (ex: "Curso", "A"). Também podem ser números (de 0 até 9) e símbolos impressos existentes em um teclado. Representado em português estruturado pelos comandos CARACTERE ou CADEIA. Os tipos de dados caractere ou cadeia são normalmente utilizados em operações de entrada e saída de dados. Caractere faz referência a um único caractere, já o cadeia quando é um conjunto de caracteres.
*   **Lógico:** Valores binários do tipo sim e não, verdadeiro ou falso, 1 e 0. Representado em português estruturado pelo comando LÓGICO. Utilizado em operações de processamento lógico através das formas dos valores .F.(ou .FALSO.) e V(ou .VERDADEIRO.). Também podem ser utilizados os valores .S.(ou .SIM.) e .N.(ou .NÃO.).

**C [Cap.3]:**
O C exige que você declare o tamanho e o tipo da variável antes de colocar qualquer coisa dentro dela. Se tentar colocar um texto numa variável declarada como número, o programa gera um erro na compilação.
*   `int` (Inteiro): Ao coletar o dado, como em um `scanf`, usa-se a abreviação d, com o operador de sequência de escape, `%d`.
*   `float` ou `double` (Real): Ao coletar o dado, como em um `scanf`, usa-se a abreviação f para float, com o operador de sequência de escape, `%f`, e lf para double, com o operador `%lf`.
*   `char` (Caractere) e String: Ao coletar o dado, como em um `scanf`, usa-se a abreviação c, com o operador de sequência de escape, `%c`. Em strings utilizamos o s, ficando com o operador `%s`.
*   `bool` (booleano)

**Python [Cap. ]:**
Em Python você não precisa declarar o tipo da variável antes de usá-la. No momento em que você guarda um valor, o interpretador descobre automaticamente o tipo da variável e aloca o espaço na memória.
`*/Se não tiver certeza sobre qual é o tipo de certo valor, o interpretador pode dizer isso a você: >>> type('Hello') class 'str'(string)/*`
`*/Se os números estiverem entre aspas, o python os considerará strings. Eles também não podem ser separados por vírgula, mas deve-se utilizar pontos./*`
*   `int` (Inteiro)
*   `float` (Real)
*   `str` (String/Texto)
*   `bool` (Lógico/Booleano)

**Diferenças C e Py:** Em C, a tipagem é estática (`int`, `char`, `float`). Em Python, a tipagem é dinâmica, o que significa que não é necessário declarar o tipo; a linguagem descobre pelo valor que você atribui.

### Constantes [Algoritmos Cap.3]
Constante é tudo o que é fixo, estável, inalterável, imutável, contínuo, de valor fixo e que é aplicado em diversos pontos de vista. Do ponto de vista computacional, que é semelhante ao matemático ou científico, constante é uma grandeza numérica fixa utilizada normalmente em uma expressão aritmética ou lógica, a qual define um valor que será inalterado na expressão, independentemente das variáveis envolvidas na operação a ser realizada.
Computacionalmente, ela pode ser classificada de três formas: implícita (quando definida dentro da linguagem com rótulos a serem utilizados nas operações de processamento), explícitas (quando definidas dentro do código pelo próprio desenvolvedor para uso do programa em uso) e internas (quando é parte da composição das equações matemáticas). As constantes seguem as mesmas regras de definição de nomes que as variáveis.

Como exemplo prático, declararemos a constante matemática pi e uma expressão matemática em Português estruturado.
```text
SAIDA = ENTRADA + 1.23 //1.23 é a constante
ou
PI = 3.14159265
SAIDA = ENTRADA + PI //PI é a constante
```
Em C, basta atribuir o valor requerido a constante na sua declaração, já em python não tem como declarar uma constante pois não tem bloqueador nativo.

### Operadores Aritméticos
Os operadores Aritméticos são responsáveis pelas operações matemáticas a serem realizadas em um computador. O termo operador é utilizado na área de programação para estabelecer as ferramentas responsáveis por executar algum tipo de ação computacional. Os operadores aritméticos são responsáveis pela execução do processamento matemático, exceto o operador de atribuição, que pode ser usado também em ações de processamento lógico. Eles são classificados em duas categorias, binários e unários. São binários quando utilizados em operações matemáticas de radiciação, exponenciação, divisão, multiplicação, adição e subtração; são unários quando atuam na inversão do estado de um valor numérico que pode ser passado de positivo para negativo ou vice-versa. Chaves e colchetes são abolidos, utilizando em seu lugar apenas os parênteses. [Manzano, Cap.3.5]
`//As regras e precedência de operadores são as mesmas utilizadas em álgebra. Veja mais no Capítulo 2.5 de “Como programar em C” ou no Capítulo 2.5 de “Pense em Python”.`

**Algoritmos [Cap. 3]:**
O símbolo seta apontada para cima é a forma oficial de representação da operação de exponenciação para a indicação de cálculos de potências e raízes.
As expressões Aritméticas são realizadas a partir do relacionamento existente entre variáveis e constantes numéricas com a utilização dos operadores aritméticos. O sinal de atribuição matemática (`=`) é substituído pela seta para a esquerda (`<-`), indicando a operação de atribuição. No exemplo de calcular a área de uma circunferência, escreveríamos como:
```text
AREA <- 3.14159265 * RAIO ↑ 2
A <- (B * H) / 2
DELTA <- B ↑ 2 - 4 * A * C
X1 <- (- B + DELTA ↑ ( 1 / 2 ) ) / ( 2 * A )
X2 <- (- B - DELTA ↑ ( 1 / 2 ) ) / ( 2 * A )
```
`*/As variáveis X1 e X2 são utilizadas para representar, respectivamente, suas equivalentes matemáticas x’ e x’’. A variável DELTA representa sua equivalente matemática Δ. A definição de DELTA (½) representa a extração da raiz quadrada DELTA./*`

**C [Cap. 2] e Python [Cap.1.4 e 2.5]:**
Alguns símbolos especiais não utilizados em álgebra estão presentes nas operações em C, como o asterisco (`*`), indicando multiplicação e o sinal de porcentagem (`%`), indicando o operador resto (modulus).
Para multiplicar a por b em álgebra, basta colocá-los lado a lado. Entretanto, se fizermos isto nesta linguagem, ab seria interpretado como um único nome.
A divisão inteira leva a um resultado inteiro, adquirindo o resto, se necessário, através do operador `%`, que só pode ser usado com operandos inteiros.

Python é bem semelhante à linguagem C ao abordar os operadores aritméticos, mas cabe adicionar o operador (`**`), que executa a exponenciação; isto é, eleva um número a uma potência, como:
```python
>>> 6 ** 2 + 6
42
```
`*/A divisão por zero é impossível e quando não definida em sistemas computacionais resulta em um erro fatal./*`
`*/Em C: Se você dividir dois números inteiros (ex: 5 / 2), o C joga fora as casas decimais e o resultado será 2. Para dar 2.5, as variáveis precisam ser float.`
`Em Python 3: O interpretador é mais moderno. Se você fizer 5 / 2, ele automaticamente devolve um float 2.5. Se você quiser que o Python jogue os decimais fora igual ao C, deve usar a divisão inteira com duas barras: 5 // 2./*`

### Lendo códigos simples e somando dois números inteiros
`*/ Um prompt diz ao usuário para realizar uma ação específica, como: printf(“Digite um número\n”);/*`

**Português Estruturado**
```text
INICIO
INTEIRO: inteiro1, inteiro2, soma
ESCREVA("Entre com o primeiro inteiro")
LEIA(inteiro1)
ESCREVA("Entre com o segundo inteiro")
LEIA(inteiro2)
soma <- inteiro1 + inteiro2
ESCREVA("A soma e ", soma)
FIM
```

**C [Cap.2]**
```c
/* Programa de soma */
#include <stdio.h>
int main() {
    int inteiro1, inteiro2, soma; /* declaração */
    printf("Entre com o primeiro inteiro\n"); /* prompt */
    scanf("%d", &inteiro1); /* lê um inteiro */
    printf("Entre com o segundo inteiro\n"); /* prompt */
    scanf("%d", &inteiro2); /* lê um inteiro */
    soma = inteiro1 + inteiro2; /* atribui soma */
    printf("A soma e %d\n", soma); /* imprime soma */
    return 0; /* indica que o programa foi bem-sucedido */
}
```
A linha 4 é uma declaração, e as expressões inteiro1, inteiro2 e soma são os nomes das variáveis, do tipo `int`, inteiro. Muitas variáveis do mesmo tipo podem estar presentes em uma declaração. As declarações devem ser colocadas depois das chaves e antes de qualquer instrução executável, para não causar erros de sintaxe/erros de compilação.
A função `scanf` recebe a entrada do dispositivo padrão. O segundo argumento começa com um e-comercial (`&`, ampersand) - chamado em C de operador de endereço - dizendo ao `scanf` o local na memória onde a variável está armazenada.
O `\n` é uma sequência de escape e posiciona o cursor no início da próxima linha.
A linha 9 contém uma instrução de atribuição usando o operador de atribuição `=`. A instrução `return 0;` passa o valor 0 de volta para o ambiente do sistema operacional, indicando que o programa foi executado satisfatoriamente.

**Python**
```python
inteiro1 = int(input("Entre com o primeiro inteiro\n"))
inteiro2 = int(input("Entre com o segundo inteiro\n"))
soma = inteiro1 + inteiro2
print(f"A soma e {soma}")
```
Ler o código da direita para a esquerda em python facilita a leitura. O comando `input()` mostra a mensagem na tela e capta o que será digitado inicialmente como string(texto). Depois, ele pega o texto digitado e converte para um número inteiro (comando `int(...)`).
Por fim, uma mensagem é mostrada na tela através de um print. O `f` significa format(formatação). Em Python, chamamos isso de f-string (Formatted String) e serve para mostrar que é necessário buscar o dado que será colocado na chave que mostra o conteúdo da variável soma, `{soma}`. Sem o f tudo é impresso como texto e as chaves também são mostradas.

### Lendo código simples com strings
Em geral, não é possível executar operações matemáticas com strings, mesmo se elas parecerem números. Mas, em python, o operador (`+`) executa uma concatenação de strings, ou seja, une as strings pelas extremidades. E o operador `*` executa a repetição com o número determinado (ex: `'Spam' * 3`).

### Conceitos sobre Memória [Deitel Cap. 2]
Nomes de variáveis correspondem realmente a locais na memória do computador. Quando a instrução `scanf("%d", &inteiro1);` é executada, o valor digitado é colocado no local da memória. Sempre que um valor é colocado em um local, o novo valor invalida o anterior naquele local (leitura destrutiva). Quando um valor é apenas lido no cálculo (como em `soma = inteiro1 + inteiro2`), o processo é chamado leitura não destrutiva.

### Operadores Relacionais
Os operadores relacionais são usados para testar condições (geralmente dentro de um if). "Fazendo uma pergunta" à CPU, e a resposta é sempre Verdadeiro ou Falso. Os operadores de igualdade possuem nível de precedência menor do que o dos operadores relacionais.
*   **Diferente:** Usa-se `!=` (Em pseudocódigo usa-se `<>`).
*   **Igualdade:** Usa-se `==` (dois sinais de igual).
Confundir o operador de atribuição com o de comparação é um erro comum. O operador de igualdade (`==`) deve ser lido como “é igual a” e o operador de atribuição (`=`) deve ser lido como “obtém” (ou recebe).

### PRINCIPAIS DIFERENÇAS ENTRE C E PYTHON, NA ESCRITA DOS CÓDIGOS
*   **Comandos de Entrada e Saída:** Em C, precisamos de `printf` e `scanf`. Em Python, o comando `input()` faz ambas as coisas simultaneamente, e a saída é `print`.
*   **Declaração e Tipos (Tipagem):** Em C, toda variável precisa ter seu tipo (`int`, `float`, `char`) declarado antes. Python é dinâmico, mas o input entra como string e precisa ser convertido explicitamente (`int()`, `float()`).
*   **Uso de Aspas:** Em C, a regra é rígida: aspas simples (`' '`) são para caractere único e aspas duplas (`" "`) para cadeias de texto. Em Python, não há distinção.

## Linguagens de Programação 
Para que um computador eletrônico funcione, ele deve ser programado. O processo de programação é uma “conversa” controlada entre um ser humano (tecnicamente preparado) e o computador. O processo de comunicação se faz com o uso de uma linguagem de programação que o computador “entenda”.

### Níveis de Linguagem de Programação [Deitel e Manzano Cap. 1]
Os programadores escrevem instruções em várias linguagens de programação, algumas entendidas diretamente pelo computador e outras que exigem passos intermediários de tradução. Centenas de linguagens computacionais estão atualmente em uso. Estas podem ser divididas em três tipos gerais: [Deitel]

*   **Linguagem de Máquina (Baixíssimo Nível):** Qualquer computador pode entender apenas sua própria linguagem de máquina. A linguagem de máquina é a "linguagem natural" de um determinado computador. Ela está relacionada intimamente com o projeto de hardware daquele computador. Geralmente as linguagens de máquina consistem em strings de números. [Deitel] É o que o processador realmente executa. São apenas 0s e 1s (binário) ou representações Hexadecimais (como o B4 09). É impossível para um ser humano escrever programas complexos assim sem errar.
*   **Linguagem de Baixo Nível (Assembly):** Em vez de usar strings de números que os computadores podiam entender diretamente, os programadores começaram a usar abreviações parecidas com palavras em inglês para representar as operações elementares de um computador. Estas abreviações formaram a base das linguagens assembly. Foram desenvolvidos programas tradutores, chamados assemblers, para converter programas em linguagem assembly para linguagem de máquina na velocidade ditada pelo computador. [Deitel] Utiliza mnemônicos (abreviações de comandos) como MOV, ADD, PUSH. É um pouco mais legível que o binário, mas ainda exige que o programador conheça cada detalhe do hardware (registradores, memória). [Manzano]
*   **Linguagem de Alto Nível:** O computador aumentou rapidamente com o advento das linguagens assembly, mas elas ainda exigiam muitas instruções para realizar mesmo as tarefas mais simples. Para acelerar o processo de programação, foram desenvolvidas linguagens de alto nível, nas quais podiam ser escritas instruções simples para realizar tarefas fundamentais. Os programas tradutores que convertiam programas de linguagem de alto nível em linguagem de máquina são chamados compiladores. [Deitel] É onde nós trabalhamos (Pascal, C, Java, Python). Utiliza palavras próximas ao inglês (if, while, print). Elas permitem focar na lógica do problema e não nos fios do computador. [Manzano]

### Gerações [Manzano Cap.1]
*   **1ª Geração (Baixíssimo Nível):** Foco no hardware. Linguagens de Máquina (binário) e Assembly. O programador precisa entender o processador.
*   **2ª Geração (Alto Nível Inicial):** Surgem as primeiras linguagens que usam palavras (inglês).
    *   FORTRAN (FORmula TRANslator): primeira linguagem de Alto Nível, usada em Cálculos científicos e engenharia.
    *   COBOL (COmmon Business Oriented Language): foi desenvolvido em 1959 por um grupo de fabricantes de computadores e usuários governamentais e industriais. O COBOL é usado principalmente para aplicações comerciais que necessitam de uma manipulação precisa e eficiente de grandes volumes de dados
    *   ALGOL e, de certa forma, BASIC.
*   **3ª Geração (Estruturadas e Multiuso):** É aqui que o curso de Algoritmos se sustenta. Introduzem o conceito de Estruturas de Controle (Repetições e Condições).
    *   Pascal: Criada especificamente para o ensino de programação (é a base do "Portugol").
    *   C / C++ / Java / Lua: Linguagens modernas e poderosas.
    *   PL/1, MODULA-2 e ADA: Outros exemplos clássicos estruturados da 3ª geração.
*   **4ª Geração (Linguagens Declarativas):** O programador não diz "como" o computador deve fazer, mas "o que" ele quer. Destacando-se a linguagem de consulta estruturada SQL.
    *   SQL: Usada para conversar com Bancos de Dados.

### Paradigmas e Estilos de Programação [Manzano Cap. 1]
*   **Procedural (ou Imperativa):** O programador dá ordens diretas ao computador (fatos e comandos em sequência). É como uma receita de bolo: "faça isso, depois aquilo".
*   **Declarativa:** Você diz o que quer, mas não como fazer. Muito comum em marcação (HTML) ou configurações.
*   **Orientada a Objetos (POO):** Tenta aproximar o código do mundo real. Em vez de apenas variáveis soltas, você cria "objetos" (ex: um objeto Carro que tem cor, modelo e a ação de dirigir).
*   **Concorrente:** Quebra a regra da sequência única. Várias coisas acontecem ao mesmo tempo (paralelismo). Como um jogo onde a música toca enquanto o personagem corre.
*   **Consulta (SQL):** Especializada em "perguntar" coisas para um banco de dados.
*   **Especificação:** Funciona como a "planta baixa" de um prédio. É para projetar antes de construir.

`*/No livro do Manzano, no final do capítulo 1, pode-se encontrar mais informações sobre as linguagens e seus respectivos usos, o modelo (estilo ou paradigma) da forma de programar computadores eletrônicos./*`

## Bibliotecas, Histórias e Ambiente

### A Biblioteca Padrão (Standard Library) do C [Deitel]
O C foi desenvolvido a partir das linguagens BCPL e B, uma linguagem independente dos hardwares. Em 1989, foi aprovado o padrão solicitado, para fornecer à linguagem uma definição inequívoca e independente de equipamento, documento conhecido como ANSI/ISO 9899:1990.
Os programas em C consistem em módulos ou elementos chamados funções. Você pode programar todas as funções de que precisa para formar um programa C, mas a maioria dos programadores C tira proveito de um excelente conjunto de funções chamado C Standard Library (Biblioteca Padrão do C).
Usar funções existentes evita reinventar a roda. No caso das funções standard do ANSI, você sabe que elas foram desenvolvidas cuidadosamente e sabe que, por estar usando funções disponíveis em praticamente todas as implementações do ANSI C, seus programas terão uma grande possibilidade de serem portáteis. A vantagem de criar suas próprias funções é que você saberá exatamente como elas funcionam. Você poderá examinar o código C. A desvantagem é o esforço demorado que se faz necessário para projetar e desenvolver novas funções.

### Compiladores, Interpretadores e Tradutores
Programadores e desenvolvedores de software possuem ferramentas de trabalho, como editores de texto, compiladores, intérpretes e tradutores, bem como a secretária e o escritor utilizam processador de textos, comumente confundido com editor, o que seria o caso de estarem envolvidos com a escrita de programas de computadores.
Assim que o projeto de um programa de computador está concluído, é necessário transformá-lo em um software. Traduzindo o projeto definido para uma linguagem de programação formal, aquela que é executada em um computador. Precisamos fazer a escrita do código de programa em uma ferramenta de edição de textos para depois passar o programa por ferramentas de tradução, interpretação e compilação, conforme a necessidade.
*   O editor de texto consiste em um programa simples que permite ao programador escrever o texto do código do programa e gravá-lo.
*   As ferramentas de tradução são programas que permitem fazer a tradução de um programa escrito em uma linguagem formal para outra, utilizando esta ferramenta para escrever um programa na linguagem que domina, reescrevendo-o na linguagem desejada.
*   As ferramentas de interpretação são programas que executam um programa-fonte escrito em uma linguagem na própria memória principal do computador, sem que ele seja executado diretamente no processador central da máquina, normalmente com rápida execução dos programas.
*   Ferramentas de compilação são programas que traduzem para uma linguagem de baixo nível (linguagem de máquina) um programa-fonte escrito em uma linguagem de alto nível, transformando o programa-fonte em um programa-objeto (escrito em linguagem de alto nível compatível com o processador em uso) e depois faz a ligação do programa-objeto com as rotinas de execução de programas do sistema operacional, tornando o programa um código executável. [Algoritmo Cap.2.4]

Ou seja, o bloco de notas é o seu editor de texto, onde sua função é salvar caracteres de texto puro em um arquivo (como .c, .py ou .txt). O tradutor é todo programa que pega um código escrito em uma linguagem (como C e Python) e o transforma em código de máquina ou assembly (os dois tipos mais famosos de tradutores são o Compilador e o Intérprete).
O compilador pega o arquivo de texto com o código inteiro, lê do início ao fim, traduz tudo de uma vez e gera um novo arquivo (o executável, como o .exe ou .out). O Intérprete não gera um arquivo executável, mas lê o código linha por linha e vai traduzindo e executando na mesma hora.
Cada um desses é uma ferramenta de trabalho, e devem ser usadas de acordo com a necessidade, sendo algumas vezes embutidas em outras ferramentas. Um exemplo disso é o VS CODE, que serve como editor de texto, intérprete e como compilador - O VS Code é um Editor de texto avançado (também chamado IDE). Ao rodar um código ele "chama" um intérprete (O python instalado no computador) ou um compilador externo (como o gcc ou clang, para gerar um executável em C).

### Os Fundamentos do Ambiente C
Todos os sistemas C são constituídos geralmente de três partes: o ambiente, a linguagem e a C Standard Library, e os programas em C normalmente passam por seis fases para serem executados. São elas: edição, pré-processamento, compilação, linking, carregamento e execução.
A primeira fase consiste na edição de um arquivo com um programa editor. O programador digita um programa, hoje em dia, usamos IDEs (Ambientes de Desenvolvimento Integrados, como o VS Code), que destacam os erros de sintaxe, para facilitar a correção da lógica. O programa é armazenado em um dispositivo de extensão .c. A seguir, o programador emite o comando de compilar o programa. O compilador traduz o programa em C para o código de linguagem de máquina(também chamado de código-objeto). Um programa pré-processador é executado automaticamente antes da fase de tradução começar. O pré-processador obedece a comandos especiais chamados diretivas do pré-processador que indicam que devem ser realizadas determinadas manipulações no programa antes da compilação (incluir outros arquivos no arquivo e substituir símbolos especiais por texto de programa).
A quarta fase é chamada linking. O código-objeto produzido pelo compilador C contém “lacunas” devido à falta de funções, referentes às funções definidas em outros locais, como nas bibliotecas padrão ou de um grupo de programadores. Um linker faz a ligação do código-objeto com o código das funções que estão faltando para produzir uma imagem executável (sem a falta de qualquer parte).
A quinta fase é chamada carregamento. Um programa deve ser colocado na memória antes que possa ser executado pela primeira vez. Isto é feito pelo carregador (rotina de carga ou loader), que apanha a imagem executável do disco e a transfere para a memória.
Finalmente, o computador, sob controle de sua CPU, executa as instruções programa, uma após a outra.

`//Determinadas funções do C recebem seus dados de entrada a partir do stdin (standard input) o fluxo de Entrada. É por este canal que os dados viajam do hardware até as variáveis na Memória RAM.`
*   Hardware clássico: Teclado.
*   Comando em C: `scanf` (ele fica "escutando" o stdin).

`stdout`(Standard Output): É o fluxo principal de Saída. Usado para enviar o resultado bem-sucedido do processamento para fora do programa.
*   Hardware clássico: Monitor/Tela.
*   Comando em C: `printf`.

`stderr`(Standard Error): É o fluxo de Erro. Também aponta para o monitor por padrão, mas é um canal VIP separado. Ele serve para que, se o seu programa travar ou tiver um erro crítico, a mensagem de socorro não se misture com os dados normais do `stdout`.

### Programação Orientada a Objetos e C++
Um superconjunto do C, o C++, foi desenvolvido por Stroustrup (St86) no Bell Laboratories, sendo um dos recursos mais atraentes a programação orientada a objetos. Objetos são basicamente componentes reutilizáveis de software que modelam itens do mundo real. Usar um projeto e método de implementação modulares e orientados a objetos pode fazer com que os grupos de desenvolvimento se tornem mais produtivos do que seria possível com técnicas convencionais de programação.

### O ambiente em Python
O python trabalha de duas maneiras: modo script e modo interativo. No modo interativo, ao atribuir um valor a uma variável e realizar um cálculo, posteriormente, com a mesma, o interpretador a avalia e exibe o resultado, mas no modo script não, você não recebe nenhuma saída. Scripts têm nomes que terminam com `.py`.

## Arquitetura, Dados e Sintaxe

### Programação de Computadores
A tarefa de se efetuar a programação de computadores se inicia com a análise de sistema, a partir do problema que será automatizado por intermédio de soluções computacionais. O programa de computador (software) é constituído primeiro na mente do programador, que deve retratar o que deseja ser feito na forma de diagrama de blocos e na documentação do código a ser executado por meio do pseudocódigo.
A partir da ideia do que necessita ser feito e da certeza de que a linha de raciocínio usada é a correta e após a documentação, passa-se à fase de codificação do programa para o computador com o uso de uma linguagem de programação (no caso, em Python ou C). A fase de codificação em português estruturada pode até ser descartada, mas é importante que o diagrama de blocos seja feito. [Algoritmos Cap. 2]

### Comentários
`/*Em C, os comentários longos podem ser indicados iniciando com (/*) e terminando com (*/), os simples, de única linha, com (//). Já em python utiliza-se, para comentários de linha única (#). Eles servem para documentar os programas e melhorar sua legibilidade, não realizando ações quando o programa é executado. Neste documento também uso barras para indicar os comentários. [Downey Cap. 2.7]*/`

### Depuração [Downey Cap.1.7 e 2.8]
Erros de programação são chamados de bugs (insetos) por causa da mariposa responsável pelos erros do computador Mark II, e o processo de rastreá-lo chama-se debugging (depuração). Há três tipos de erros que podem ocorrer em um programa: erros de sintaxe, erros de tempo de execução e erros semânticos.
*   **Erros de sintaxe:** A “sintaxe” refere-se à estrutura de um programa e suas respectivas regras. Por exemplo, os parênteses devem vir em pares correspondentes, então `(1 + 2` é um erro de sintaxe. Erros de sintaxe impedem a execução do programa.
*   **Erro de tempo de execução:** Este tipo de erro não aparece até que o programa seja executado, e geralmente indicam que algo excepcional (e ruim) aconteceu.
*   **Erro semântico:** É um erro relacionado ao significado. Ele executa sem gerar mensagens de erro, mas o programa acontecerá de um modo diferente do que deveria. Identificá-los pode ser complicado pois é necessário, a partir da saída do programa, compreender o que ele está fazendo.

### Algoritmos Computacionais [Manzano Cap. 2]
A palavra algoritmos vem do latim, dos termos algarismos ou algorithmos, que estão associados à ideia de algarismos por influência do idioma grego a partir do termo arithmós, que remete a números. Na esfera matemática, está associada a um processo de cálculo; encadeamento das ações necessárias ao cumprimento de uma tarefa; processo efetivo, que produz uma solução para um problema em um número finito de etapas. Na ciência da computação, está associada a um conjunto das regras e procedimentos lógicos perfeitamente definidos que levam à solução de um problema em um número finito de etapas.
O termo algoritmo, do ponto de vista computacional, pode ser entendido como regras formais, sequenciais e bem definidas a partir do entendimento lógico de um problema a ser resolvido por um programador com o objetivo de transformá-lo em um programa que seja possível de ser tratado e executado por um computador, em que dados de entrada são transformados em dados de saída.

`/*As bases que norteiam o processo da programação de computadores vêm das mesmas ideias estudadas e apresentadas por Charles Babbage com a máquina analítica e da programação idealizada por sua assistente, Ada Augusta Byron King, considerada pioneira na programação de computadores.*/`

### Lógica na programação de computadores
As ferramentas gráficas utilizadas no projeto lógico da programação podem ser os diagramas de blocos, diagramas de quadros ou Chapin. O uso dessas ferramentas possibilita demonstrar de forma concreta a linha de raciocínio lógico (que é um elemento abstrato) que o profissional de desenvolvimento usou para escrever um programa de computador.
As ferramentas textuais (pseudocódigos ou metalinguagens) permitem descrever de forma simples e sem o rigor técnico de uma linguagem de programação formal as etapas que o programa de computador deve executar, desde que essas etapas estejam definidas e delineadas como uma das ferramentas gráficas existes. Podendo ser usado com base na técnica chamada Program Design Language (PDL), que é uma linguagem de projeto, não de programação. No Brasil, essa técnica é normalmente utilizada com os nomes português estruturado ou portugol.
A técnica mais importante no projeto da lógica de programas baseada em algoritmos denomina-se programação estruturada ou programação modular, usando uma metodologia de projeto que agiliza a codificação da escrita da programação, facilita a depuração da leitura, permite a verificação de possíveis falhas apresentadas pelos programas, dentre muitas outras coisas.

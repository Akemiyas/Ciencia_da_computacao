## O Computador
É um dispositivo capaz de realizar cálculos e tomar decisões lógicas com uma velocidade de milhões ou mesmo bilhões de vezes mais rápida do que os seres humanos, podendo realizar dezenas de milhões de operações aritméticas por segundo.

Os computadores processam dados sob o controle de conjuntos de instruções chamados programas de computador. Estes programas conduzem o computador através de um conjunto ordenado de ações especificado por pessoas chamadas programadores de computador. [Deitel Cap.1]

A palavra computador origina-se do termo em latim computatore, um substantivo masculino que significa “aquele ou aquilo que efetua cálculos”. O computador eletrônico, como se conhece atualmente, origina-se das ideias estabelecidas pelo cientista, matemático e filósofo inglês Charles Babbage, que em 1834 apresentou os fundamentos da máquina analítica, considerada precursora dos modernos computadores [Mazano Cap.1]

### O Hardware e Software
Os vários dispositivos (como teclado, tela, discos, memória e unidades de processamento) que constituem um sistema computacional são chamados de hardware. Os programas executados em um computador e sistemas são chamados de software. [Deitel Cap. 1]

## A Organização dos computadores [Deitel e Manzano Cap.1]

### Os componentes de um computador eletrônico:
*   **Unidade de Entrada (Input Unit):** A unidade de entrada é a seção de "recepção" do computador. Atualmente a maioria das informações é fornecida aos computadores através de teclados como os de máquinas de escrever, mas também pode ser representado pelos periféricos scanner, mouse, câmeras de vídeo, arquivos, sensores de movimento, entre outros componentes.
*   **Unidade Central de Processamento (Central Processing Unit, CPU):** responsável pelo controle das operações de entrada e de saída de um computador e por todo o controle operacional, sendo o “cérebro” e o “sistema nervoso” de um computador. Ela é subdividida em três componentes auxiliares:
    `/*Assim como a memória principal refere-se a memória RAM e ROM, a CPU se refere às suas três subdivisões, elas (A memória principal e a CPU) não existem em si mesmas.*/`
    *   **Unidade Lógica e Aritmética (Arithmetic and Logic Unit, ALU):** Executa todas as contas matemáticas e testes lógicos programados (soma, subtração...). Realiza cálculos e toma decisões. Operadores Aritméticos usados na ALU: `[ + ]` = Adição. `[ - ]` = Subtração. `[ * ]` = Multiplicação. `[ / ]` = Divisão. `[ ^ ]` = Potenciação. `[MOD]` ou `[%]` = Resto da divisão.
    *   **Registradores:** São pequenas memórias ultra-rápidas dentro do processador. Eles seguram os dados que a ULA(ALU) está usando naquele exato milissegundo, ou seja, possuem alta performance de velocidade na execução de instruções de processamento aritmético ou lógico.
    *   **Unidade de Controle(UC):** É responsável por interpretar cada linha de instrução escrita e decide o que deve ser feito a seguir. Dependendo da instrução executada, esse componente faz o desvio do controle para a unidade lógica ou unidade aritmética ou, ainda, envia dados para componentes externos à CPU.
*   **Unidade de Saída(Output Unit):** É responsável pela apresentação de dados e/ou informações que tenham sido processados na memória principal ou que estejam armazenados na memória secundária do computador. Esse tipo de componente pode ser representado pelos periféricos: monitores de vídeo, impressoras, arquivos, entre outros.
*   **Memória Principal/Unidade de Memória:** A unidade de memória é a seção de "armazenamento" do computador e é chamada frequentemente de memória, memória principal ou memória primária. Formada principalmente pelos componentes de memórias RAM e ROM.
    *   **Memória RAM:** Podemos dizer que é o espaço das variáveis (Quando você declara uma variável, você está reservando um "endereço" na RAM para guardar um dado temporariamente). Esse tipo de operação é muito rápida porque é realizada por um conjunto de circuitos lógicos, mas é uma memória volátil e os dados são perdidos ao desligar ou reiniciar o computador.
    *   **Memória ROM:** Usada pela CPU quando se inicializa o computador, buscando o sistema operacional instalado na memória secundária, a qual gerencia as funções de trabalho e permite usar o computador de forma mais fácil. A memória ROM não pode ser alterada ou regravada como ocorre com os dados e instruções da memória RAM, pois nela estão gravadas as características definidas pelo fabricante do computador em uso.
*   **Memória Secundária:** Conhecida memória de massa, armazena dados em longo prazo, mesmo quando o computador estiver desligado. Essa memória possui, normalmente, acesso lento. São exemplos os periféricos de armazenamento: discos rígidos (HDs, pendrives, cartões de memória, discos ópticos, SSDs (solid-state drive), entre outros.

## O Ciclo do Processamento [Manzano Cap. 3]
Para transformar o Dado em Informação, seguimos o fluxo:
*   **Entrada:** Receber os dados brutos, podendo armazená-los na memória principal para realizar algum tipo de processamento ou armazenar na memória secundária para usar futuramente.
*   **Processamento:** Organizar, calcular ou comparar esses dados. É quando o computador, por meio de um programa (software) executado em sua memória primária, faz a transformação dos dados entrados ou previamente armazenados em sua memória secundária, tornando-os elementos que possam ser usados como fontes de informação para o mundo externo.
*   **Saída:** Entregar a informação pronta para o uso. O computador envia os dados processados na memória principal ou armazenados na memória secundária para o mundo externo, transformando os dados processados em fontes de informação.

`/*O Software(seu algoritmo) dá ordens ao Hardware.`
`O processamento de um diagrama de blocos, por exemplo, ocorre dentro da ULA. A UC lê meu código, busca os valores das variáveis na RAM, entrega para a ULA fazer o cálculo e devolve o resultado para a RAM ou para a Saída(monitor).*/`

## Unidades de Medidas Computacionais [Manzano Cap. 1]

### Bit e Byte
*   **Bit (binary digit):** É a menor unidade de informação. Sua representação física é um impulso elétrico (“1”, ligado) ou a ausência dele (“0”, desligado). Dizemos que ele é base 2 (binário) porque ele tem apenas duas possibilidades de estado. Os valores binários são eletronicamente usados pelo computador para representar estados eletromagnéticos dos circuitos que compõem a sua estrutura funcional e, assim, possibilitam representar dados do mundo exterior, além de estabelecer as bases de funcionamento da própria máquina. O computador tem a capacidade de utilizar dados e informações do mundo exterior e representá-los de forma binária em seus circuitos e memórias. Assim, os dados básicos existentes no mundo exterior, como dados numéricos e alfabéticos, incluindo os símbolos de pontuação, possuem um valor binário particular para os representar no computador.
*   **Byte (octeto):** É um conjunto de 8 bits agrupados. É a unidade necessária para representar um caractere (uma letra, um número ou um símbolo). Tomando por base o valor numérico 2 referente à base de operação interna de um computador eletrônico (o bit) e elevando esse valor ao expoente 8 referente à quantidade de bits de um byte (2^8), obtém-se o valor 256, que é a quantidade máxima de caracteres que podem ser usados em um computador eletrônico como definido junto a tabela ASCII.
    *   Se você tem 1 bit, tem 2 combinações: (0), (1).
    *   Se você tem 2 bits, tem 4 combinações: (00), (01), (10), (11).
    *   Se você tem 8 bits (um byte), a matemática é 2*2*2*2*2*2*2*2 = 2^8

## A Evolução da Codificação [Manzano Cap. 1]
(BAUDOT X ASCII)
*   **O código de Baudot:** utilizava 5 bits (2^5). Isso resultava em apenas 32 combinações. Era limitado e mal dava para as letras do alfabeto e alguns controles.
*   **ASCII Padrão:** Utiliza 7 bits (embora armazenado em 1 byte). Define os primeiros 128 caracteres (0 a 127). É o "idioma universal" dos computadores para letras inglesas, números e sinais básicos.
*   **ASCII Estendido:** Utiliza 8 bits para alcançar 256 combinações (2^8). Os códigos de 128 a 255 são usados para caracteres especiais, acentuação e símbolos gráficos, variando conforme a região ou fabricante.

## Diferença entre Dado e Informação [Manzano Cap.1]
*   **Dado:** É a matéria-prima bruta. Isolado, ele não possui um significado completo ou útil para uma tomada de decisão.
Exemplos: "35", "João", "Solteiro".
*   **Informação:** É o dado processado, organizado e com contexto. É o que gera conhecimento.
Exemplo: "João tem 35 anos e é solteiro" (Perfil de um cliente).

`*/* A Composição do Hexadecimal (Base 16)*`
`*0, 1, 2, 3, 4, 5, 6, 7, 8, 9 (Valores de 0 a 9)*`
`*A (vale 10), B (vale 11), C (vale 12), D (vale 13), E (vale 14), F (vale 15) \*/*`

## O que é um programa? [Downey Cap. 1]
Um programa é uma sequência de instruções que especifica como executar uma operação de computação. A operação de computação pode ser algo matemático, como solucionar um sistema de equações ou encontrar as raízes de um polinômio, mas também pode ser uma operação de computação simbólica, como a busca e a substituição de textos em um documento; ou algo gráfico, como o processamento de uma imagem ou a reprodução de um vídeo.

Os detalhes parecem diferentes em linguagens diferentes, mas algumas instruções básicas aparecem em quase todas as linguagens:
*   **Entrada:** Receber dados do teclado, de um arquivo, da rede ou de algum outro dispositivo.
*   **Saída:** Exibir dados na tela, salvá-los em um arquivo, enviá-los pela rede etc.
*   **Matemática:** Executar operações matemáticas básicas como adição e multiplicação.
*   **Execução condicional:** Verificar a existência de certas condições e executar o código adequado.
*   **Repetição:** Executar várias vezes alguma ação, normalmente com algumas variações.

## Processamento em Lotes (Batch Processing), Multiprogramação e Tempo Compartilhado (Timesharing) [Deitel Cap. 1]
Os primeiros computadores eram capazes de realizar apenas um trabalho ou tarefa de cada vez. Esta forma de funcionamento de computadores é chamada frequentemente de processamento em lotes de usuário único. O computador executa um único programa de cada vez enquanto processa dados em grupos ou lotes (batches).

`*/Nesses primeiros sistemas, geralmente os usuários enviavam suas tarefas ao centro computacional em pilhas de cartões perfurados. Freqüentemente os usuários precisavam esperar horas antes que as saídas impressas fossem levadas para seus locais de trabalho. /*`

A multiprogramação envolve as "operações" simultâneas de muitas tarefas do computador — o computador compartilha seus recursos entre as tarefas que exigem sua atenção.

`*/Com os primeiros sistemas de multiprogramação, os usuários ainda enviavam seus programas em pilhas de cartões perfurados e esperavam horas ou dias para obter os resultados./*`

Timesharing é um caso especial de multiprogramação no qual os usuários podem ter acesso ao computador através de dispositivos de entrada/saída ou terminais. Em um sistema computacional típico de timesharing, pode haver dezenas de usuários compartilhando o computador ao mesmo tempo.

`*/Na realidade o computador não atende a todos os usuários simultaneamente. Em vez disso, ele executa uma pequena parte da tarefa de um usuário e então passa a fazer a tarefa do próximo usuário. O computador faz isto tão rapidamente que pode executar o serviço de cada usuário várias vezes por segundo. Assim, parece que as tarefas dos usuários estão sendo executadas simultaneamente./*`

## Computação Pessoal, Computação Distribuída e Computação Cliente/Servidor [Deitel Cap. 1]
Em 1997, a Apple Computer tornou popular o fenômeno da computação pessoal. Computadores tornaram-se suficientemente baratos para serem comprados para uso pessoal ou comercial. Em 1981, a IBM, a maior vendedora de computadores do mundo, criou o IBM PC (Personal Computer, computador pessoal).

Embora os primeiros computadores pessoais não fossem suficientemente poderosos para serem compartilhados por vários usuários, esses equipamentos podiam ser ligados entre si em redes de computadores, algumas vezes através de linhas telefônicas e algumas vezes em redes locais de organizações. Isto levou ao fenômeno da computação distribuída, na qual a carga de trabalho computacional de uma organização, em vez de ser realizada exclusivamente em uma instalação central de informática, é distribuída em redes para os locais (sites) nos quais o trabalho real da organização é efetuado. Os computadores pessoais eram suficientemente poderosos para manipular as exigências computacionais de cada usuário em particular e as tarefas básicas de comunicações de passar as informações eletronicamente de um lugar para outro.

`*/Os computadores pessoais mais poderosos de hoje são tão poderosos quanto os equipamentos de milhões de dólares de apenas uma década atrás. Os equipamentos desktop (computadores de mesa) mais poderosos — chamados workstations ou estações de trabalho — fornecem capacidades enormes a usuários isolados. As informações são compartilhadas facilmente em redes de computadores onde alguns deles, os chamados servidores de arquivos (file servers), oferecem um depósito comum de programas e dados que podem ser usados pelos computadores clientes (clients) distribuídos ao longo da rede, daí o termo computação cliente/servidor. O C e o C ++ tornaram-se as linguagens preferidas de programação para a criação de software destinado a sistemas operacionais, redes de computadores e aplicações distribuídas cliente/servidor./*`

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

## O Computador[cite: 1]
É um dispositivo capaz de realizar cálculos e tomar decisões lógicas com uma velocidade de milhões ou mesmo bilhões de vezes mais rápida do que os seres humanos, podendo realizar dezenas de milhões de operações aritméticas por segundo.[cite: 1]

Os computadores processam dados sob o controle de conjuntos de instruções chamados programas de computador.[cite: 1] Estes programas conduzem o computador através de um conjunto ordenado de ações especificado por pessoas chamadas programadores de computador.[cite: 1] [Deitel Cap.1][cite: 1]

A palavra computador origina-se do termo em latim computatore, um substantivo masculino que significa “aquele ou aquilo que efetua cálculos”.[cite: 1] O computador eletrônico, como se conhece atualmente, origina-se das ideias estabelecidas pelo cientista, matemático e filósofo inglês Charles Babbage, que em 1834 apresentou os fundamentos da máquina analítica, considerada precursora dos modernos computadores [Mazano Cap.1][cite: 1]

### O Hardware e Software[cite: 1]
Os vários dispositivos (como teclado, tela, discos, memória e unidades de processamento) que constituem um sistema computacional são chamados de hardware.[cite: 1] Os programas executados em um computador e sistemas são chamados de software.[cite: 1] [Deitel Cap. 1][cite: 1]

## A Organização dos computadores [Deitel e Manzano Cap.1][cite: 1]

### Os componentes de um computador eletrônico:[cite: 1]
*   **Unidade de Entrada (Input Unit):** A unidade de entrada é a seção de "recepção" do computador.[cite: 1] Atualmente a maioria das informações é fornecida aos computadores através de teclados como os de máquinas de escrever, mas também pode ser representado pelos periféricos scanner, mouse, câmeras de vídeo, arquivos, sensores de movimento, entre outros componentes.[cite: 1]
*   **Unidade Central de Processamento (Central Processing Unit, CPU):** responsável pelo controle das operações de entrada e de saída de um computador e por todo o controle operacional, sendo o “cérebro” e o “sistema nervoso” de um computador.[cite: 1] Ela é subdividida em três componentes auxiliares:[cite: 1]
    `/*Assim como a memória principal refere-se a memória RAM e ROM, a CPU se refere às suas três subdivisões, elas (A memória principal e a CPU) não existem em si mesmas.*/`[cite: 1]
    *   **Unidade Lógica e Aritmética (Arithmetic and Logic Unit, ALU):** Executa todas as contas matemáticas e testes lógicos programados (soma, subtração...).[cite: 1] Realiza cálculos e toma decisões.[cite: 1] Operadores Aritméticos usados na ALU: `[ + ]` = Adição.[cite: 1] `[ - ]` = Subtração.[cite: 1] `[ * ]` = Multiplicação.[cite: 1] `[ / ]` = Divisão.[cite: 1] `[ ^ ]` = Potenciação.[cite: 1] `[MOD]` ou `[%]` = Resto da divisão.[cite: 1]
    *   **Registradores:** São pequenas memórias ultra-rápidas dentro do processador.[cite: 1] Eles seguram os dados que a ULA(ALU) está usando naquele exato milissegundo, ou seja, possuem alta performance de velocidade na execução de instruções de processamento aritmético ou lógico.[cite: 1]
    *   **Unidade de Controle(UC):** É responsável por interpretar cada linha de instrução escrita e decide o que deve ser feito a seguir.[cite: 1] Dependendo da instrução executada, esse componente faz o desvio do controle para a unidade lógica ou unidade aritmética ou, ainda, envia dados para componentes externos à CPU.[cite: 1]
*   **Unidade de Saída(Output Unit):** É responsável pela apresentação de dados e/ou informações que tenham sido processados na memória principal ou que estejam armazenados na memória secundária do computador.[cite: 1] Esse tipo de componente pode ser representado pelos periféricos: monitores de vídeo, impressoras, arquivos, entre outros.[cite: 1]
*   **Memória Principal/Unidade de Memória:** A unidade de memória é a seção de "armazenamento" do computador e é chamada frequentemente de memória, memória principal ou memória primária.[cite: 1] Formada principalmente pelos componentes de memórias RAM e ROM.[cite: 1]
    *   **Memória RAM:** Podemos dizer que é o espaço das variáveis (Quando você declara uma variável, você está reservando um "endereço" na RAM para guardar um dado temporariamente).[cite: 1] Esse tipo de operação é muito rápida porque é realizada por um conjunto de circuitos lógicos, mas é uma memória volátil e os dados são perdidos ao desligar ou reiniciar o computador.[cite: 1]
    *   **Memória ROM:** Usada pela CPU quando se inicializa o computador, buscando o sistema operacional instalado na memória secundária, a qual gerencia as funções de trabalho e permite usar o computador de forma mais fácil.[cite: 1] A memória ROM não pode ser alterada ou regravada como ocorre com os dados e instruções da memória RAM, pois nela estão gravadas as características definidas pelo fabricante do computador em uso.[cite: 1]
*   **Memória Secundária:** Conhecida memória de massa, armazena dados em longo prazo, mesmo quando o computador estiver desligado.[cite: 1] Essa memória possui, normalmente, acesso lento.[cite: 1] São exemplos os periféricos de armazenamento: discos rígidos (HDs, pendrives, cartões de memória, discos ópticos, SSDs (solid-state drive), entre outros.[cite: 1]

## O Ciclo do Processamento [Manzano Cap. 3][cite: 1]
Para transformar o Dado em Informação, seguimos o fluxo:[cite: 1]
*   **Entrada:** Receber os dados brutos, podendo armazená-los na memória principal para realizar algum tipo de processamento ou armazenar na memória secundária para usar futuramente.[cite: 1]
*   **Processamento:** Organizar, calcular ou comparar esses dados.[cite: 1] É quando o computador, por meio de um programa (software) executado em sua memória primária, faz a transformação dos dados entrados ou previamente armazenados em sua memória secundária, tornando-os elementos que possam ser usados como fontes de informação para o mundo externo.[cite: 1]
*   **Saída:** Entregar a informação pronta para o uso.[cite: 1] O computador envia os dados processados na memória principal ou armazenados na memória secundária para o mundo externo, transformando os dados processados em fontes de informação.[cite: 1]

`/*O Software(seu algoritmo) dá ordens ao Hardware.`[cite: 1]
`O processamento de um diagrama de blocos, por exemplo, ocorre dentro da ULA. A UC lê meu código, busca os valores das variáveis na RAM, entrega para a ULA fazer o cálculo e devolve o resultado para a RAM ou para a Saída(monitor).*/`[cite: 1]

## Unidades de Medidas Computacionais [Manzano Cap. 1][cite: 1]

### Bit e Byte[cite: 1]
*   **Bit (binary digit):** É a menor unidade de informação.[cite: 1] Sua representação física é um impulso elétrico (“1”, ligado) ou a ausência dele (“0”, desligado).[cite: 1] Dizemos que ele é base 2 (binário) porque ele tem apenas duas possibilidades de estado.[cite: 1] Os valores binários são eletronicamente usados pelo computador para representar estados eletromagnéticos dos circuitos que compõem a sua estrutura funcional e, assim, possibilitam representar dados do mundo exterior, além de estabelecer as bases de funcionamento da própria máquina.[cite: 1] O computador tem a capacidade de utilizar dados e informações do mundo exterior e representá-los de forma binária em seus circuitos e memórias.[cite: 1] Assim, os dados básicos existentes no mundo exterior, como dados numéricos e alfabéticos, incluindo os símbolos de pontuação, possuem um valor binário particular para os representar no computador.[cite: 1]
*   **Byte (octeto):** É um conjunto de 8 bits agrupados.[cite: 1] É a unidade necessária para representar um caractere (uma letra, um número ou um símbolo).[cite: 1] Tomando por base o valor numérico 2 referente à base de operação interna de um computador eletrônico (o bit) e elevando esse valor ao expoente 8 referente à quantidade de bits de um byte (2^8), obtém-se o valor 256, que é a quantidade máxima de caracteres que podem ser usados em um computador eletrônico como definido junto a tabela ASCII.[cite: 1]
    *   Se você tem 1 bit, tem 2 combinações: (0), (1).[cite: 1]
    *   Se você tem 2 bits, tem 4 combinações: (00), (01), (10), (11).[cite: 1]
    *   Se você tem 8 bits (um byte), a matemática é 2*2*2*2*2*2*2*2 = 2^8[cite: 1]

## A Evolução da Codificação [Manzano Cap. 1][cite: 1]
(BAUDOT X ASCII)[cite: 1]
*   **O código de Baudot:** utilizava 5 bits (2^5).[cite: 1] Isso resultava em apenas 32 combinações.[cite: 1] Era limitado e mal dava para as letras do alfabeto e alguns controles.[cite: 1]
*   **ASCII Padrão:** Utiliza 7 bits (embora armazenado em 1 byte).[cite: 1] Define os primeiros 128 caracteres (0 a 127).[cite: 1] É o "idioma universal" dos computadores para letras inglesas, números e sinais básicos.[cite: 1]
*   **ASCII Estendido:** Utiliza 8 bits para alcançar 256 combinações (2^8).[cite: 1] Os códigos de 128 a 255 são usados para caracteres especiais, acentuação e símbolos gráficos, variando conforme a região ou fabricante.[cite: 1]

## Diferença entre Dado e Informação [Manzano Cap.1][cite: 1]
*   **Dado:** É a matéria-prima bruta.[cite: 1] Isolado, ele não possui um significado completo ou útil para uma tomada de decisão.[cite: 1]
Exemplos: "35", "João", "Solteiro".[cite: 1]
*   **Informação:** É o dado processado, organizado e com contexto.[cite: 1] É o que gera conhecimento.[cite: 1]
Exemplo: "João tem 35 anos e é solteiro" (Perfil de um cliente).[cite: 1]

`*/* A Composição do Hexadecimal (Base 16)*`[cite: 1]
`*0, 1, 2, 3, 4, 5, 6, 7, 8, 9 (Valores de 0 a 9)*`[cite: 1]
`*A (vale 10), B (vale 11), C (vale 12), D (vale 13), E (vale 14), F (vale 15) \*/*`[cite: 1]

## O que é um programa? [Downey Cap. 1][cite: 1]
Um programa é uma sequência de instruções que especifica como executar uma operação de computação.[cite: 1] A operação de computação pode ser algo matemático, como solucionar um sistema de equações ou encontrar as raízes de um polinômio, mas também pode ser uma operação de computação simbólica, como a busca e a substituição de textos em um documento; ou algo gráfico, como o processamento de uma imagem ou a reprodução de um vídeo.[cite: 1]

Os detalhes parecem diferentes em linguagens diferentes, mas algumas instruções básicas aparecem em quase todas as linguagens:[cite: 1]
*   **Entrada:** Receber dados do teclado, de um arquivo, da rede ou de algum outro dispositivo.[cite: 1]
*   **Saída:** Exibir dados na tela, salvá-los em um arquivo, enviá-los pela rede etc.[cite: 1]
*   **Matemática:** Executar operações matemáticas básicas como adição e multiplicação.[cite: 1]
*   **Execução condicional:** Verificar a existência de certas condições e executar o código adequado.[cite: 1]
*   **Repetição:** Executar várias vezes alguma ação, normalmente com algumas variações.[cite: 1]

## Processamento em Lotes (Batch Processing), Multiprogramação e Tempo Compartilhado (Timesharing) [Deitel Cap. 1][cite: 1]
Os primeiros computadores eram capazes de realizar apenas um trabalho ou tarefa de cada vez.[cite: 1] Esta forma de funcionamento de computadores é chamada frequentemente de processamento em lotes de usuário único.[cite: 1] O computador executa um único programa de cada vez enquanto processa dados em grupos ou lotes (batches).[cite: 1]

`*/Nesses primeiros sistemas, geralmente os usuários enviavam suas tarefas ao centro computacional em pilhas de cartões perfurados. Freqüentemente os usuários precisavam esperar horas antes que as saídas impressas fossem levadas para seus locais de trabalho. /*`[cite: 1]

A multiprogramação envolve as "operações" simultâneas de muitas tarefas do computador — o computador compartilha seus recursos entre as tarefas que exigem sua atenção.[cite: 1]

`*/Com os primeiros sistemas de multiprogramação, os usuários ainda enviavam seus programas em pilhas de cartões perfurados e esperavam horas ou dias para obter os resultados./*`[cite: 1]

Timesharing é um caso especial de multiprogramação no qual os usuários podem ter acesso ao computador através de dispositivos de entrada/saída ou terminais.[cite: 1] Em um sistema computacional típico de timesharing, pode haver dezenas de usuários compartilhando o computador ao mesmo tempo.[cite: 1]

`*/Na realidade o computador não atende a todos os usuários simultaneamente. Em vez disso, ele executa uma pequena parte da tarefa de um usuário e então passa a fazer a tarefa do próximo usuário. O computador faz isto tão rapidamente que pode executar o serviço de cada usuário várias vezes por segundo. Assim, parece que as tarefas dos usuários estão sendo executadas simultaneamente./*`[cite: 1]

## Computação Pessoal, Computação Distribuída e Computação Cliente/Servidor [Deitel Cap. 1][cite: 1]
Em 1997, a Apple Computer tornou popular o fenômeno da computação pessoal.[cite: 1] Computadores tornaram-se suficientemente baratos para serem comprados para uso pessoal ou comercial.[cite: 1] Em 1981, a IBM, a maior vendedora de computadores do mundo, criou o IBM PC (Personal Computer, computador pessoal).[cite: 1]

Embora os primeiros computadores pessoais não fossem suficientemente poderosos para serem compartilhados por vários usuários, esses equipamentos podiam ser ligados entre si em redes de computadores, algumas vezes através de linhas telefônicas e algumas vezes em redes locais de organizações.[cite: 1] Isto levou ao fenômeno da computação distribuída, na qual a carga de trabalho computacional de uma organização, em vez de ser realizada exclusivamente em uma instalação central de informática, é distribuída em redes para os locais (sites) nos quais o trabalho real da organização é efetuado.[cite: 1] Os computadores pessoais eram suficientemente poderosos para manipular as exigências computacionais de cada usuário em particular e as tarefas básicas de comunicações de passar as informações eletronicamente de um lugar para outro.[cite: 1]

`*/Os computadores pessoais mais poderosos de hoje são tão poderosos quanto os equipamentos de milhões de dólares de apenas uma década atrás. Os equipamentos desktop (computadores de mesa) mais poderosos — chamados workstations ou estações de trabalho — fornecem capacidades enormes a usuários isolados. As informações são compartilhadas facilmente em redes de computadores onde alguns deles, os chamados servidores de arquivos (file servers), oferecem um depósito comum de programas e dados que podem ser usados pelos computadores clientes (clients) distribuídos ao longo da rede, daí o termo computação cliente/servidor. O C e o C ++ tornaram-se as linguagens preferidas de programação para a criação de software destinado a sistemas operacionais, redes de computadores e aplicações distribuídas cliente/servidor./*`[cite: 1]

## Linguagens de Programação[cite: 1]
Para que um computador eletrônico funcione, ele deve ser programado.[cite: 1] O processo de programação é uma “conversa” controlada entre um ser humano (tecnicamente preparado) e o computador.[cite: 1] O processo de comunicação se faz com o uso de uma linguagem de programação que o computador “entenda”.[cite: 1]

### Níveis de Linguagem de Programação [Deitel e Manzano Cap. 1][cite: 1]
Os programadores escrevem instruções em várias linguagens de programação, algumas entendidas diretamente pelo computador e outras que exigem passos intermediários de tradução.[cite: 1] Centenas de linguagens computacionais estão atualmente em uso.[cite: 1] Estas podem ser divididas em três tipos gerais: [Deitel][cite: 1]

*   **Linguagem de Máquina (Baixíssimo Nível):** Qualquer computador pode entender apenas sua própria linguagem de máquina.[cite: 1] A linguagem de máquina é a "linguagem natural" de um determinado computador.[cite: 1] Ela está relacionada intimamente com o projeto de hardware daquele computador.[cite: 1] Geralmente as linguagens de máquina consistem em strings de números. [Deitel][cite: 1] É o que o processador realmente executa.[cite: 1] São apenas 0s e 1s (binário) ou representações Hexadecimais (como o B4 09).[cite: 1] É impossível para um ser humano escrever programas complexos assim sem errar.[cite: 1]
*   **Linguagem de Baixo Nível (Assembly):** Em vez de usar strings de números que os computadores podiam entender diretamente, os programadores começaram a usar abreviações parecidas com palavras em inglês para representar as operações elementares de um computador.[cite: 1] Estas abreviações formaram a base das linguagens assembly.[cite: 1] Foram desenvolvidos programas tradutores, chamados assemblers, para converter programas em linguagem assembly para linguagem de máquina na velocidade ditada pelo computador. [Deitel][cite: 1] Utiliza mnemônicos (abreviações de comandos) como MOV, ADD, PUSH.[cite: 1] É um pouco mais legível que o binário, mas ainda exige que o programador conheça cada detalhe do hardware (registradores, memória). [Manzano][cite: 1]
*   **Linguagem de Alto Nível:** O computador aumentou rapidamente com o advento das linguagens assembly, mas elas ainda exigiam muitas instruções para realizar mesmo as tarefas mais simples.[cite: 1] Para acelerar o processo de programação, foram desenvolvidas linguagens de alto nível, nas quais podiam ser escritas instruções simples para realizar tarefas fundamentais.[cite: 1] Os programas tradutores que convertiam programas de linguagem de alto nível em linguagem de máquina são chamados compiladores. [Deitel][cite: 1] É onde nós trabalhamos (Pascal, C, Java, Python).[cite: 1] Utiliza palavras próximas ao inglês (if, while, print).[cite: 1] Elas permitem focar na lógica do problema e não nos fios do computador. [Manzano][cite: 1]

### Gerações [Manzano Cap.1][cite: 1]
*   **1ª Geração (Baixíssimo Nível):** Foco no hardware.[cite: 1] Linguagens de Máquina (binário) e Assembly.[cite: 1] O programador precisa entender o processador.[cite: 1]
*   **2ª Geração (Alto Nível Inicial):** Surgem as primeiras linguagens que usam palavras (inglês).[cite: 1]
    *   FORTRAN (FORmula TRANslator): primeira linguagem de Alto Nível, usada em Cálculos científicos e engenharia.[cite: 1]
    *   COBOL (COmmon Business Oriented Language): foi desenvolvido em 1959 por um grupo de fabricantes de computadores e usuários governamentais e industriais.[cite: 1] O COBOL é usado principalmente para aplicações comerciais que necessitam de uma manipulação precisa e eficiente de grandes volumes de dados[cite: 1]
    *   ALGOL e, de certa forma, BASIC.[cite: 1]
*   **3ª Geração (Estruturadas e Multiuso):** É aqui que o curso de Algoritmos se sustenta.[cite: 1] Introduzem o conceito de Estruturas de Controle (Repetições e Condições).[cite: 1]
    *   Pascal: Criada especificamente para o ensino de programação (é a base do "Portugol").[cite: 1]
    *   C / C++ / Java / Lua: Linguagens modernas e poderosas.[cite: 1]
    *   PL/1, MODULA-2 e ADA: Outros exemplos clássicos estruturados da 3ª geração.[cite: 1]
*   **4ª Geração (Linguagens Declarativas):** O programador não diz "como" o computador deve fazer, mas "o que" ele quer.[cite: 1] Destacando-se a linguagem de consulta estruturada SQL.[cite: 1]
    *   SQL: Usada para conversar com Bancos de Dados.[cite: 1]

### Paradigmas e Estilos de Programação [Manzano Cap. 1][cite: 1]
*   **Procedural (ou Imperativa):** O programador dá ordens diretas ao computador (fatos e comandos em sequência).[cite: 1] É como uma receita de bolo: "faça isso, depois aquilo".[cite: 1]
*   **Declarativa:** Você diz o que quer, mas não como fazer.[cite: 1] Muito comum em marcação (HTML) ou configurações.[cite: 1]
*   **Orientada a Objetos (POO):** Tenta aproximar o código do mundo real.[cite: 1] Em vez de apenas variáveis soltas, você cria "objetos" (ex: um objeto Carro que tem cor, modelo e a ação de dirigir).[cite: 1]
*   **Concorrente:** Quebra a regra da sequência única.[cite: 1] Várias coisas acontecem ao mesmo tempo (paralelismo).[cite: 1] Como um jogo onde a música toca enquanto o personagem corre.[cite: 1]
*   **Consulta (SQL):** Especializada em "perguntar" coisas para um banco de dados.[cite: 1]
*   **Especificação:** Funciona como a "planta baixa" de um prédio.[cite: 1] É para projetar antes de construir.[cite: 1]

`*/No livro do Manzano, no final do capítulo 1, pode-se encontrar mais informações sobre as linguagens e seus respectivos usos, o modelo (estilo ou paradigma) da forma de programar computadores eletrônicos./*`[cite: 1]

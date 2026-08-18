# Ciencia_da_computacao
Anotações e conteúdos aprendidos/estudados no curso de Ciência da Computação.

ANOTAÇÕES DOS LIVROS “PENSE EM PYTHON”, “ALGORITMOS” e “COMO PROGRAMAR EM C”
SUMÁRIO DESTE DOCUMENTO:

* [1. O Computador e Arquitetura de Hardware](#-o-computador-e-arquitetura-de-hardware)
  * [Hardware e Software](#hardware-e-software)
  * [Organização dos Computadores (CPU, ALU, Registradores)](#organização-dos-computadores-cpu-alu-registradores)
  * [Ciclo de Processamento e Unidades de Medida](#ciclo-de-processamento-e-unidades-de-medidas-computacionais)
* [2. Conceitos Gerais de Programação](#2-conceitos-gerais-de-programação)
  * [Evolução, Níveis e Paradigmas das Linguagens](#linguagens-de-programação)
  * [Compiladores, Interpretadores e Ambientes (C e Python)](#compiladores-interpretadores-e-tradutores)
  * [Tipos de Erro e Depuração](#depuração)
* [3. Fundamentos Práticos e Sintaxe (C vs. Python)](#3-fundamentos-práticos-e-sintaxe-c-vs-python)
  * [Entrada, Saída e Fluxos de Dados](#entrada-e-saída-de-dados)
  * [Tipos de Dados, Variáveis e Memória RAM](#tipos-de-dados-e-variáveis)
  * [Operadores Aritméticos e Relacionais](#operadores-aritméticos)
  * [Diferenças Chave de Escrita entre C e Python](#principais-diferenças-entre-c-e-python-na-escrita-dos-códigos)
* [4. Exercícios Resolvidos](#4-exercícios-resolvidos)
  * [Cálculo da Área do Círculo](#cálculo-da-área-de-um-círculo)
  * [Cálculo do Salário de um Professor](#cálculo-do-salário-de-um-professor)
  * [Exercícios de Fixação e Tabela de Palavras Reservadas](#exercícios-de-fixação)
* [5. Tópicos Avançados e Práticas Recomendadas](#5-tópicos-avançados-e-práticas-recomendadas)
  * [Estruturas de Dados (Vetores, Listas, Dicionários, JSON)](#listas-e-dicionários)
  * [Ponteiros e Passagem de Parâmetros](#ponteiros-)
  * [Práticas Recomendáveis e Dicas de Portabilidade](#práticas-recomendáveis-de-programação)

---
## 1. O Computador e Arquitetura de Hardware
é um dispositivo capaz de realizar cálculos e tomar decisões lógicas com uma velocidade de milhões ou mesmo bilhões de vezes mais rápida do que os seres humanos, podendo realizar dezenas de milhões de operações aritméticas por segundo.
Os computadores processam dados sob o controle de conjuntos de instruções chamados programas de computador. Estes programas conduzem o computador através de um conjunto ordenado de ações especificado por pessoas chamadas programadores de computador. [Deitel Cap.1]
A palavra computador origina-se do termo em latim computatore, um substantivo masculino que significa “aquele ou aquilo que efetua cálculos”.
	O computador eletrônico, como se conhece atualmente, origina-se das ideias estabelecidas pelo cientista, matemático e filósofo inglês Charles Babbage, que em 1834 apresentou os fundamentos da máquina analítica, considerada precursora dos modernos computadores [Mazano Cap.1]
O Hardware e Software 
Os vários dispositivos (como teclado, tela, discos, memória e unidades de processamento) que constituem um sistema computacional são chamados de hardware. Os programas executados em um computador e sistemas são chamados de software. [Deitel Cap. 1]  
A Organização dos computadores [Deitel e Manzano Cap.1]
Os componentes de um computador eletrônico:


Unidade de Entrada (Input Unit): A unidade de entrada é a seção de "recepção" do computador. Atualmente a maioria das informações é fornecida aos computadores através de teclados como os de máquinas de escrever, mas também pode ser representado pelos periféricos scanner, mouse, câmeras de vídeo, arquivos, sensores de movimento, entre outros componentes.
 
Unidade Central de Processamento (Central Processing Unit, CPU): responsável pelo controle das operações de entrada e de saída de um computador e por todo o controle operacional, sendo o “cérebro” e o “sistema nervoso” de um computador. Ela é subdividida em três componentes auxiliares:

/*Assim como a memória principal refere-se a memória RAM e ROM, a CPU se refere às suas três subdivisões, elas (A memória principal e a CPU) não existem em si mesmas.*/

Unidade Lógica e Aritmética (Arithmetic and Logic Unit, ALU): Executa todas as contas matemáticas e testes lógicos programados (soma, subtração...). Realiza cálculos e toma decisões.

Operadores Aritméticos usados na ALU:
[ + ] = Adição.
[ - ] = Subtração.
[ * ] = Multiplicação.
[ / ] = Divisão.
[ ^ ] = Potenciação.
[MOD] ou [%] = Resto da divisão.

Registradores: São pequenas memórias ultra-rápidas dentro do processador. Eles seguram os dados que a ULA(ALU) está usando naquele exato milissegundo, ou seja, possuem alta performance de velocidade na execução de instruções de processamento aritmético ou lógico. 
 
Unidade de Controle(UC): É responsável por interpretar cada linha de instrução escrita e decide o que deve ser feito a seguir. Dependendo da instrução executada, esse componente faz o desvio do controle para a unidade lógica ou unidade aritmética ou, ainda, envia dados para componentes externos à CPU.  

Unidade de Saída(Output Unit): É responsável pela apresentação de dados e/ou informações que tenham sido processados na memória principal ou que estejam armazenados na memória secundária do computador. Esse tipo de componente pode ser representado pelos periféricos: monitores de vídeo, impressoras, arquivos, entre outros. 

Memória Principal/Unidade de Memória: A unidade de memória é a seção de "armazenamento" do computador e é chamada frequentemente de memória, memória principal ou memória primária. Formada principalmente pelos componentes de memórias RAM e ROM.    

Memória RAM: Podemos dizer que é o espaço das variáveis (Quando você declara uma variável, você está reservando um "endereço" na RAM para guardar um dado temporariamente). Esse tipo de operação é muito rápida porque é realizada por um conjunto de circuitos lógicos, mas é uma memória volátil e os dados são perdidos ao desligar ou reiniciar o computador.

Memória ROM: Usada pela CPU quando se inicializa o computador, buscando o sistema operacional instalado na memória secundária, a qual gerencia as funções de trabalho e permite usar o computador de forma mais fácil. A memória ROM não pode ser alterada ou regravada como ocorre com os dados e instruções da memória RAM, pois nela estão gravadas as características definidas pelo fabricante do computador em uso.  

Memória Secundária: Conhecida memória de massa, armazena dados em longo prazo, mesmo quando o computador estiver desligado. Essa memória possui, normalmente, acesso lento. São exemplos os periféricos de armazenamento: discos rígidos (HDs, pendrives, cartões de memória, discos ópticos, SSDs (solid-state drive), entre outros. 
O Ciclo do Processamento [Manzano Cap. 3]
Para transformar o Dado em Informação, seguimos o fluxo:
Entrada: Receber os dados brutos, podendo armazená-los na memória principal para realizar algum tipo de processamento ou armazenar na memória secundária para usar futuramente.
Processamento: Organizar, calcular ou comparar esses dados. É quando o computador, por meio de um programa (software) executado em sua memória primária, faz a transformação dos dados entrados ou previamente armazenados em sua memória secundária, tornando-os elementos que possam ser usados como fontes de informação para o mundo externo. 
Saída: Entregar a informação pronta para o uso. O computador envia os dados processados na memória principal ou armazenados na memória secundária para o mundo externo, transformando os dados processados em fontes de informação.

/*O Software(seu algoritmo) dá ordens ao Hardware.

O processamento de um diagrama de blocos, por exemplo, ocorre dentro da ULA. A UC lê meu código, busca os valores das variáveis na RAM, entrega para a ULA fazer o cálculo e devolve o resultado para a RAM ou para a Saída(monitor).*/

Unidades de Medidas Computacionais [Manzano Cap. 1]
Bit e Byte

Bit (binary digit): É a menor unidade de informação. Sua representação física é um impulso elétrico (“1”, ligado) ou a ausência dele (“0”, desligado). Dizemos que ele é base 2 (binário) porque ele tem apenas duas possibilidades de estado. Os valores binários são eletronicamente usados pelo computador para representar estados eletromagnéticos dos circuitos que compõem a sua estrutura funcional e, assim, possibilitam representar dados do mundo exterior, além de estabelecer as bases de funcionamento da própria máquina. O computador tem a capacidade de utilizar dados e informações do mundo exterior e representá-los de forma binária em seus circuitos e memórias. Assim, os dados básicos existentes no mundo exterior, como dados numéricos e alfabéticos, incluindo os símbolos de pontuação, possuem um valor binário particular para os representar no computador. 

Byte (octeto): É um conjunto de 8 bits agrupados. É a unidade necessária para representar um caractere (uma letra, um número ou um símbolo). Tomando por base o valor numérico 2 referente à base de operação interna de um computador eletrônico (o bit) e elevando esse valor ao expoente 8 referente à quantidade de bits de um byte (2^8), obtém-se o valor 256, que é a quantidade máxima de caracteres que podem ser usados em um computador eletrônico como definido junto a tabela ASCII . 

Se você tem 1 bit, tem 2 combinações: (0), (1).
Se você tem 2 bits, tem 4 combinações: (00), (01), (10), (11).
Se você tem 8 bits (um byte), a matemática é 2*2*2*2*2*2*2*2 = 2^8 
A Evolução da Codificação [Manzano Cap. 1]
(BAUDOT X ASCII)

O código de Baudot: utilizava 5 bits (2^5). Isso resultava em apenas 32 combinações. Era limitado e mal dava para as letras do alfabeto e alguns controles.

ASCII Padrão: Utiliza 7 bits (embora armazenado em 1 byte). Define os primeiros 128 caracteres (0 a 127). É o "idioma universal" dos computadores para letras inglesas, números e sinais básicos.

ASCII Estendido: Utiliza 8 bits para alcançar 256 combinações (2^8). Os códigos de 128 a 255 são usados para caracteres especiais, acentuação e símbolos gráficos, variando conforme a região ou fabricante.
 Diferença entre Dado e Informação [Manzano Cap.1]
Dado: É a matéria-prima bruta. Isolado, ele não possui um significado completo ou útil para uma tomada de decisão.
Exemplos: "35", "João", "Solteiro".

Informação: É o dado processado, organizado e com contexto. É o que gera conhecimento.
Exemplo: "João tem 35 anos e é solteiro" (Perfil de um cliente).


*/\* A Composição do Hexadecimal (Base 16)*

*0, 1, 2, 3, 4, 5, 6, 7, 8, 9 (Valores de 0 a 9)*

*A (vale 10), B (vale 11), C (vale 12), D (vale 13), E (vale 14), F (vale 15) \*/*
O que é um programa? [Downey Cap. 1]
Um programa é uma sequência de instruções que especifica como executar uma operação de computação. A operação de computação pode ser algo matemático, como solucionar um sistema de equações ou encontrar as raízes de um polinômio, mas também pode ser uma operação de computação simbólica, como a busca e a substituição de textos em um documento; ou algo gráfico, como o processamento de uma imagem ou a reprodução de um vídeo. 
Os detalhes parecem diferentes em linguagens diferentes, mas algumas instruções básicas aparecem em quase todas as linguagens:
 Entrada: Receber dados do teclado, de um arquivo, da rede ou de algum outro dispositivo. 
	Saída: Exibir dados na tela, salvá-los em um arquivo, enviá-los pela rede etc. 
	Matemática: Executar operações matemáticas básicas como adição e multiplicação. 
	Execução condicional: Verificar a existência de certas condições e executar o código adequado. 
	Repetição: Executar várias vezes alguma ação, normalmente com algumas variaç
 (Batch Processing), Multiprogramação e Tempo Compartilhado (Timesharing) [Deitel Cap. 1]
Os primeiros computadores eram capazes de realizar apenas um trabalho ou tarefa de cada vez. Esta forma de funcionamento de computadores é chamada frequentemente de processamento em lotes de usuário único. O computador executa um único programa de cada vez enquanto processa dados em grupos ou lotes (batches).
*/Nesses primeiros sistemas, geralmente os usuários enviavam suas tarefas ao centro
computacional em pilhas de cartões perfurados. Freqüentemente os usuários precisavam esperar horas antes que as saídas impressas fossem levadas para seus locais de trabalho. /* 
A multiprogramação envolve as "operações" simultâneas de muitas tarefas do computador — o computador compartilha seus recursos entre as tarefas que exigem sua atenção. 
*/Com os primeiros sistemas de multiprogramação, os usuários ainda enviavam seus programas em pilhas de cartões perfurados e esperavam horas ou dias para obter os resultados./*
Timesharing é um caso especial de multiprogramação no qual os usuários podem ter acesso ao computador através de dispositivos de entrada/saída ou terminais. Em um sistema computacional típico de timesharing, pode haver dezenas de usuários compartilhando o computador ao mesmo tempo.
*/Na realidade o computador não atende a todos os usuários simultaneamente. Em vez disso, ele executa uma pequena parte da tarefa de um usuário e então passa a fazer a tarefa do próximo usuário. O computador faz isto tão rapidamente que pode executar o serviço de cada usuário várias vezes por segundo. Assim, parece que as tarefas dos usuários estão sendo executadas simultaneamente./*
Computação Pessoal, Computação Distribuída e Computação Cliente/Servidor [Deitel Cap. 1]
Em 1997, a Apple Computer tornou popular o fenômeno da computação pessoal. Computadores tornaram-se suficientemente baratos para serem comprados para uso pessoal ou comercial. Em 1981, a IBM, a maior vendedora de computadores do mundo, criou o IBM PC (Personal Computer, computador pessoal). 
Embora os primeiros computadores pessoais não fossem suficientemente poderosos para serem compartilhados por vários usuários, esses equipamentos podiam ser ligados entre si em redes de computadores, algumas vezes através de linhas telefônicas e algumas vezes em redes locais de organizações. Isto levou ao fenômeno da computação distribuída, na qual a carga de trabalho computacional de uma organização, em vez de ser realizada exclusivamente em uma instalação central de informática, é distribuída em redes para os locais (sites) nos quais o trabalho real da organização é efetuado. Os computadores pessoais eram suficientemente poderosos para manipular as exigências computacionais de cada usuário em particular e as tarefas básicas de comunicações de passar as informações eletronicamente de um lugar para outro. 
*/Os computadores pessoais mais poderosos de hoje são tão poderosos quanto os equipamentos de milhões de dólares de apenas uma década atrás. Os equipamentos desktop (computadores de mesa) mais poderosos — chamados workstations ou estações de trabalho — fornecem capacidades enormes a usuários isolados. As informações são compartilhadas facilmente em redes de computadores onde alguns deles, os chamados servidores de arquivos (file servers), oferecem um depósito comum de programas e dados que podem ser usados pelos computadores clientes (clients) distribuídos ao longo da rede, daí o termo computação cliente/servidor. O C e o C ++ tornaram-se as linguagens preferidas de programação para a criação de software destinado a sistemas operacionais, redes de computadores e aplicações distribuídas cliente/servidor./* 
 Linguagens de Programação
	Para que um computador eletrônico funcione, ele deve ser programado. O processo de programação é uma “conversa” controlada entre um ser humano (tecnicamente preparado) e o computador. O processo de comunicação se faz com o uso de uma linguagem de programação que o computador “entenda”.
Níveis de Linguagem de Programação [Deitel e Manzano Cap. 1]
Os programadores escrevem instruções em várias linguagens de programação, algumas entendidas diretamente pelo computador e outras que exigem passos intermediários de tradução. Centenas de linguagens computacionais estão atualmente em uso. Estas podem ser divididas em três tipos gerais: [Deitel]

Linguagem de Máquina (Baixíssimo Nível): 
Qualquer computador pode entender apenas sua própria linguagem de máquina. A linguagem de máquina é a "linguagem natural" de um determinado computador. Ela está relacionada intimamente com o projeto de hardware daquele computador. Geralmente as linguagens de máquina consistem em strings de números. [Deitel]
	É o que o processador realmente executa. São apenas 0s e 1s (binário) ou representações Hexadecimais (como o B4 09). É impossível para um ser humano escrever programas complexos assim sem errar.

Linguagem de Baixo Nível (Assembly): 
	Em vez de usar strings de números que os computadores podiam entender diretamente, os programadores começaram a usar abreviações parecidas com palavras em inglês para representar as operações elementares de um computador. Estas abreviações formaram a base das linguagens assembly. Foram desenvolvidos programas tradutores, chamados assemblers, para converter programas em linguagem assembly para linguagem de máquina na velocidade ditada pelo computador. [Deitel]
	Utiliza mnemônicos (abreviações de comandos) como MOV, ADD, PUSH. É um pouco mais legível que o binário, mas ainda exige que o programador conheça cada detalhe do hardware (registradores, memória). [Manzano]

Linguagem de Alto Nível: 
O computador aumentou rapidamente com o advento das linguagens assembly, mas elas ainda exigiam muitas instruções para realizar mesmo as tarefas mais simples. Para acelerar o processo de programação, foram desenvolvidas linguagens de alto nível, nas quais podiam ser escritas instruções simples para realizar tarefas fundamentais. Os programas tradutores que convertiam programas de linguagem de alto nível em linguagem de máquina são chamados compiladores. [Deitel]
É onde nós trabalhamos (Pascal, C, Java, Python). Utiliza palavras próximas ao inglês (if, while, print). Elas permitem focar na lógica do problema e não nos fios do computador. [Manzano]
 Gerações [Manzano Cap.1]
1ª Geração (Baixíssimo Nível): Foco no hardware. Linguagens de Máquina (binário) e Assembly. O programador precisa entender o processador.
2ª Geração (Alto Nível Inicial): Surgem as primeiras linguagens que usam palavras (inglês). 
FORTRAN (FORmula TRANslator): primeira linguagem de Alto Nível, usada em Cálculos científicos e engenharia.
COBOL(COmmon Business Oriented Language): foi desenvolvido em 1959 por um grupo de fabricantes de computadores e usuários governamentais e industriais. O COBOL é usado principalmente para aplicações comerciais que necessitam de uma manipulação precisa e eficiente de grandes volumes de dados 
ALGOL e, de certa forma, BASIC.
3ª Geração (Estruturadas e Multiuso): É aqui que o curso de Algoritmos se sustenta. Introduzem o conceito de Estruturas de Controle (Repetições e Condições).
Pascal: Criada especificamente para o ensino de programação (é a base do "Portugol").
C / C++ / Java / Lua: Linguagens modernas e poderosas.
PL/1, MODULA-2 e ADA: Outros exemplos clássicos estruturados da 3ª geração. 

4ª Geração (Linguagens Declarativas): O programador não diz "como" o computador deve fazer, mas "o que" ele quer. Destacando-se a linguagem de consulta estruturada SQL.
SQL: Usada para conversar com Bancos de Dados.
Paradigmas e Estilos de Programação
[Manzano Cap. 1]

Procedural (ou Imperativa): O programador dá ordens diretas ao computador (fatos e comandos em sequência). É como uma receita de bolo: "faça isso, depois aquilo".*
Declarativa: Você diz o que quer, mas não como fazer. Muito comum em marcação (HTML) ou configurações.
Orientada a Objetos (POO): Tenta aproximar o código do mundo real. Em vez de apenas variáveis soltas, você cria "objetos" (ex: um objeto Carro que tem cor, modelo e a ação de dirigir).
Concorrente: Quebra a regra da sequência única. Várias coisas acontecem ao mesmo tempo (paralelismo). Como um jogo onde a música toca enquanto o personagem corre.
Consulta (SQL): Especializada em "perguntar" coisas para um banco de dados.
Especificação: Funciona como a "planta baixa" de um prédio. É para projetar antes de construir.


*/No livro do Manzano, no final do capítulo 1, pode-se encontrar mais informações sobre as linguagens e seus respectivos usos, o modelo (estilo ou paradigma) da forma de programar computadores eletrônicos./*






















Bibliotecas, Histórias e Ambiente
A Biblioteca Padrão (Standard Library) do C 
[Deitel]
O C foi desenvolvido a partir das linguagens BCPL e B, uma linguagem independente dos hardwares. Em 1989, foi aprovado o padrão solicitado, para fornecer à linguagem uma definição inequívoca e independente de equipamento, documento conhecido como ANSI/ISO 9899:1990. 
Os programas em C consistem em módulos ou elementos chamados funções. Você pode programar todas as funções de que precisa para formar um programa C, mas a maioria dos programadores C tira proveito de um excelente conjunto de funções chamado C Standard Library (Biblioteca Padrão do C). 
Usar funções existentes evita reinventar a roda. No caso das funções standard do ANSI, você sabe que elas foram desenvolvidas cuidadosamente e sabe que, por estar usando funções disponíveis em praticamente todas as implementações do ANSI C, seus programas terão uma grande possibilidade de serem portáteis.
A vantagem de criar suas próprias funções é que você saberá exatamente como elas funcionam. Você poderá examinar o código C. A desvantagem é o esforço demorado que se faz necessário para projetar e desenvolver novas funções.
Compiladores, Interpretadores e Tradutores
	Programadores e desenvolvedores de software possuem ferramentas de trabalho, como editores de texto, compiladores, intérpretes e tradutores, bem como a secretária e o escritor utilizam processador de textos, comumente confundido com editor, o que seria o caso de estarem envolvidos com a escrita de programas de computadores.
	Assim que o projeto de um programa de computador está concluído, é necessário transformá-lo em um software. Traduzindo o projeto definido para uma linguagem de programação formal, aquela que é executada em um computador. Precisamos fazer a escrita do código de programa em uma ferramenta de edição de textos para depois passar o programa por ferramentas de tradução, interpretação e compilação, conforme a necessidade. 
	O editor de texto consiste em um programa simples que permite ao programador escrever o texto do código do programa e gravá-lo.
	As ferramentas de tradução são programas que permitem fazer a tradução de um programa escrito em uma linguagem formal para outra, utilizando esta ferramenta para escrever um programa na linguagem que domina, reescrevendo-o na linguagem desejada.
	As ferramentas de interpretação são programas que executam um programa-fonte escrito em uma linguagem na própria memória principal do computador, sem que ele seja executado diretamente no processador central da máquina, normalmente com rápida execução dos programas.
	Ferramentas de compilação são programas que traduzem para uma linguagem de baixo nível (linguagem de máquina) um programa-fonte escrito em uma linguagem de alto nível, transformando o programa-fonte em um programa-objeto (escrito em linguagem de alto nível compatível com o processador em uso) e depois faz a ligação do programa-objeto com as rotinas de execução de programas do sistema operacional, tornando o programa um código executável. [Algoritmo Cap.2.4]
	Ou seja, o bloco de notas é o seu editor de texto, onde sua função é salvar caracteres de texto puro em um arquivo (como .c, .py ou .txt). O tradutor é todo programa que pega um código escrito em uma linguagem (como C e Python) e o transforma em código de máquina ou assembly (os dois tipos mais famosos de tradutores são o Compilador e o Intérprete).
O compilador pega o arquivo de texto com o código inteiro, lê do início ao fim, traduz tudo de uma vez e gera um novo arquivo (o executável, como o .exe ou .out).
O Intérprete não gera um arquivo executável, mas lê o código linha por linha e vai traduzindo e executando na mesma hora.
Cada um desses é uma ferramenta de trabalho, e devem ser usadas de acordo com a necessidade, sendo algumas vezes embutidas em outras ferramentas. Um exemplo disso é o VS CODE, que serve como editor de texto, intérprete e como compilador -  O VS Code é um Editor de texto avançado (também chamado IDE). Ao rodar um código ele "chama" um intérprete (O python instalado no computador) ou um compilador externo (como o gcc ou clang, para gerar um executável em C).
Os Fundamentos do Ambiente C

Todos os sistemas C são constituídos geralmente de três partes: o ambiente, a linguagem e a C Standard Library, e os programas em C normalmente passam por seis fases para serem executados. São elas: edição, pré-processamento,compilação,linking,carregamento e execução.
A primeira fase consiste na edição de um arquivo com um programa editor. O programador digita um programa , hoje em dia, usamos IDEs (Ambientes de Desenvolvimento Integrados, como o VS Code), que destacam os erros de sintaxe, para facilitar a correção da lógica. O programa é armazenado em um dispositivo de extensão .c. A seguir, o programador emite o comando de compilar o programa. O compilador traduz o programa em C para o código de linguagem de máquina(também chamado de código-objeto). Um programa pré-processador é executado automaticamente antes da fase de tradução começar. O pré-processador obedece a comandos especiais chamados diretivas do pré-processador que indicam que devem ser realizadas determinadas manipulações no programa antes da compilação (incluir outros arquivos no arquivo e substituir símbolos especiais por texto de programa).
A quarta fase é chamada linking. O código-objeto produzido pelo compilador C contém “lacunas”” devido à falta de funções, referentes às funções definidas em outros locais, como nas bibliotecas padrão ou de um grupo de programadores. Um linker faz a ligação do código-objeto com o código das funções que estão faltando para produzir uma imagem executável (sem a falta de qualquer parte).
A quinta fase é chamada carregamento. Um programa deve ser colocado na memória antes que possa ser executado pela primeira vez. Isto é feito pelo carregador (rotina de carga ou loader), que apanha a imagem executável do disco e a transfere para a memória.
Finalmente, o computador, sob controle de sua CPU, executa as instruções programa, uma após a outra.
//Determinadas funções do C recebem seus dados de entrada a partir do stdin (standard input) o fluxo de Entrada. É por este canal que os dados viajam do hardware até as variáveis na Memória RAM.
Hardware clássico: Teclado.
Comando em C: scanf (ele fica "escutando" o stdin).
stdout(Standard Output): É o fluxo principal de Saída. Usado para enviar o resultado bem-sucedido do processamento para fora do programa.
Hardware clássico: Monitor/Tela.
Comando em C: printf.
stderr(Standard Error): É o fluxo de Erro. Também aponta para o monitor por padrão, mas é um canal VIP separado. Ele serve para que, se o seu programa travar ou tiver um erro crítico, a mensagem de socorro não se misture com os dados normais do stdout. 





Programação Orientada a Objetos e C++
	Um superconjunto do C, o C++, foi desenvolvido por Stroustrup (St86) no Bell Laboratories, sendo um dos recursos mais atraentes a programação orientada a objetos.
Objetos são basicamente componentes reutilizáveis de software que modelam itens do mundo real. Usar um projeto e método de implementação modulares e orientados a objetos pode fazer com que os grupos de desenvolvimento se tornem mais produtivos do que seria possível com técnicas convencionais de programação.
O ambiente em Python
O python trabalha de duas maneiras: modo script e modo interativo. No modo interativo, ao atribuir um valor a uma variável e realizar um cálculo, posteriormente, com a mesma, o interpretador a avalia e exibe o resultado, mas no modo script não, você não recebe nenhuma saída.	
Scripts têm nomes que terminam com .py.




































Arquitetura, Dados e Sintaxe
Programação de Computadores
	A tarefa de se efetuar a programação de computadores se inicia com a análise de sistema, a partir do problema que será automatizado por intermédio de soluções computacionais.O programa de computador (software) é constituído primeiro na mente do programador, que deve retratar o que deseja ser feito na forma de diagrama de blocos e na documentação do código a ser executado por meio do pseudocódigo.
	A partir da ideia do que necessita ser feito e da certeza de que a linha de raciocínio usada é a correta e após a documentação, passa-se à fase de codificação do programa para o computador com o uso de uma linguagem de programação (no caso, em Python ou C). A fase de codificação em português estruturada pode até ser descartada, mas é importante que o diagrama de blocos seja feito.[Algoritmos Cap. 2]
	Comentários

	/*Em C, os comentários longos podem ser indicados iniciando com (/*) e terminando com (*/), os simples, de única linha, com (//). Já em python utiliza-se, para comentários de linha única (#). 
Eles servem para documentar os programas e melhorar sua legibilidade, não realizando ações quando o programa é executado. Neste documento também uso barras para indicar os comentários.[Downey Cap. 2.7]*/
Depuração [Downey Cap.1.7 e 2.8]
Erros de programação são chamados de bugs (insetos) por causa da mariposa responsável pelos erros do computador Mark II, e o processo de rastreá-lo chama-se debugging (depuração).
Há três tipos de erros que podem ocorrer em um programa: erros de sintaxe, erros de tempo de execução e erros semânticos.
Erros de sintaxe: 
A “sintaxe” refere-se à estrutura de um programa e suas respectivas regras. Por exemplo, os parênteses devem vir em pares correspondentes, então (1 + 2 é um erro de sintaxe.
Erros de sintaxe impedem a execução do programa.
Erro de tempo de execução:
Este tipo de erro não aparece até que o programa seja executado, e geralmente indicam que algo excepcional (e ruim) aconteceu.
Erro semântico:
É um erro relacionado ao significado. Ele executa sem gerar mensagens de erro, mas o programa acontecerá de um modo diferente do que deveria. Identificá-los pode ser complicado pois é necessário, a partir da saída do programa, compreender o que ele está fazendo.
Algoritmos Computacionais [Manzano Cap. 2]
	A palavra algoritmos vem do latim, dos termos algarismos ou algorithmos, que estão associados à ideia de algarismos por influência do idioma grego a partir do termo arithmós, que remete a números. Na esfera matemática, está associada a um processo de cálculo; encadeamento das ações necessárias ao cumprimento de uma tarefa; processo efetivo, que produz uma solução para um problema em um número finito de etapas. Na ciência da computação, está associada a um conjunto das regras e procedimentos lógicos perfeitamente definidos que levam à solução de um problema em um número finito de etapas.
	O termo algoritmo, do ponto de vista computacional, pode ser entendido como regras formais, sequenciais e bem definidas a partir do entendimento lógico de um problema a ser resolvido por um programador com o objetivo de transformá-lo em um programa que seja possível de ser tratado e executado por um computador, em que dados de entrada são transformados em dados de saída.
	/*As bases que norteiam o processo da programação de computadores vêm das mesmas ideias estudadas e apresentadas por Charles Babbage com a máquina analítica e da programação idealizada por sua assistente, Ada Augusta Byron King, considerada pioneira na programação de computadores.*/
Lógica na programação de computadores
As ferramentas gráficas utilizadas no projeto lógico da programação podem ser os diagramas de blocos, diagramas de quadros ou Chapin. O uso dessas ferramentas possibilita demonstrar de forma concreta a linha de raciocínio lógico (que é um elemento abstrato) que o profissional de desenvolvimento usou para escrever um programa de computador.
As ferramentas textuais (pseudocódigos ou metalinguagens) permitem descrever de forma simples e sem o rigor técnico de uma linguagem de programação formal as etapas que o programa de computador deve executar, desde que essas etapas estejam definidas e delineadas como uma das ferramentas gráficas existes. Podendo ser usado com base na técnica chamada Program Design Language (PDL), que é uma linguagem de projeto, não de programação. No Brasil, essa técnica é normalmente utilizada com os nomes português estruturado ou portugol.
A técnica mais importante no projeto da lógica de programas baseada em algoritmos denomina-se programação estruturada ou programação modular, usando uma metodologia de projeto que agiliza a codificação da escrita da programação, facilita a depuração da leitura, permite a verificação de possíveis falhas apresentadas pelos programas, dentre muitas outras coisas. 
	A diferença do início dos programas
 Algoritmos [Cap. 2]
	No pseudocódigo ou fluxograma, a lógica exige demarcar onde as coisas começam e terminam para não gerar loops infinitos. Demarcada pelas palavras INÍCIO e FIM ou pela figura oval no topo do fluxograma:

	*/Apesar de utilizamos textos em português ao digitar pseudocódigos, toda linguagem de programação formal, para ser aceita mundialmente como ferramenta de trabalho, é sempre definida em inglês.E, se escrito manualmente, nunca deve conter letras minúsculas, e o zero deve vir acompanhado de um traço perpendicular, semelhante ao símbolo de conjunto vazio./*

C [Cap.2]
O C é composto por funções, sendo a principal a main(), os parênteses após a palavra indicam que é um bloco de construção do programa, ou seja, uma função. Todos os programas em C começam a ser executados pela função main. 
O bloco é uma unidade importante e são mostrados através das chaves {, para começar o corpo e } para terminar.

Python [Cap. 1]
	As três primeiras linhas ao iniciar o interpretador do Python contém informações sobre o interpretador e o sistema operacional em que está sendo executado. Após conferir também o número da versão basta fazer um teste de soma, pressionar Enter e observar se o resultado é exibido.
	Dado os fatos, podemos dizer que para inicializar um programa em python basta o interpretador abrir o arquivo .py e começar a ler freneticamente da linha 1 para baixo, executando o que vê pela frente. 
Entrada e Saída de dados
Para o programa ser útil, ele precisa receber dados do usuário (Entrada) e devolver um resultado (Saída). 
Algoritmos [Cap. 2]
No pseudocódigo, usamos os comandos LEIA() para capturar e ESCREVA() para   mostrar na tela.
//A lista com os comandos em português estruturado estarão no final da página.
C [Cap.2] 
O C exige saber o tipo de dado que está entrando ou saindo. Usamos a biblioteca <stdio.h> porque o receber e devolver não faz parte da linguagem de programação C, mas são funções desta biblioteca. 
Saída (printf): Imprime na tela. O f significa format.
printf("Bem-vindo ao C!\n"); 
Imprime na tela a string de caracteres limitada pelas aspas. A linha inteira, completa, é chamada de instrução, e toda instrução deve terminar com um ponto e vírgula (;).
O \n, apesar de estar entre as aspas, não é impresso pois é está com uma backlash, caractere de escape. Veja as sequências de escape no final da página.
Entrada (scanf): Lê do teclado. Exige o uso do & (e comercial) para apontar para o endereço físico da variável na memória RAM.
/*Por não fazerem parte da linguagem, o compilador não pode encontrar um erro de digitação em printf e scanf, ele apenas abre espaço no programa objeto para uma “chamada” à função da biblioteca. O compilador não sabe onde as funções da biblioteca se encontram, mas o linker sabe, e ele que localizará o erro.*/



Python [Cap.2 e 5] 
O Python simplifica o processo unindo a mensagem de tela e a captura de dados no mesmo comando, sem precisar do endereço de memória (&).
Saída: print()
>>> print(‘Hello, World!’) 
Hello, World 
	As aspas marcam o começo e o fim do texto a ser exibido, elas não aparecem no resultado. Os parênteses indicam que o print é uma função.
Entrada: input() //Encontrada no capítulo 5
Python
idade = input("Digite sua idade: ") # Faz a saída da pergunta e a entrada do dado de uma vez
Tipos de Dados e Variáveis [Algoritmos Cap. 3]
Os dados são elementos do mundo exterior que representam, dentro de um computador digital, as informações manipuladas pelos seres humanos. Eles podem ser classificados em três tipos primitivos ou tipos básicos: numéricos, caracteres, e lógicos. 
Variável é tudo que está sujeito a variações, que é incerto, instável ou inconstante. É necessário saber o tipo de dado para depois fazer seu armazenamento adequado, e armazenado o dado desejado, ele pode ser utilizado e processado a qualquer momento. Como uma "gaveta" na Memória RAM com uma etiqueta (nome) e um formato específico, usada para guardar um dado.      
  
O nome de uma variável é utilizado para sua identificação e representação em um programa de computador e deve seguir algumas regras: 
Podem utilizar um ou mais caracteres, limitando-se a restrições da própria linguagem formal de programação em uso (no caso do português estruturado, essa restrição não existe) .
O primeiro caractere de identificação do nome de uma var. não pode ser numérico ou símbolo gráfico, sempre deve ser alfabético (os demais caracteres podem ser alfanuméricos).
Não pode haver espaços em branco. Caso deseje, pode-se utilizar o caractere de separação “_” underline.
Jamais deve ser definida com o mesmo nome de uma palavra que represente um dos comandos ou instruções de uma linguagem de programação de computadores. (Veja a lista das palavras reservadas em C, Python e português estruturado nas páginas finais.)
Não pode ser algum rótulo que já tenha sido usado para identificar o nome de um programa ou mesmo de outra variável. Um nome torna-se exclusivo no programa em que foi definido. (Em C, temos escopos diferentes e as variáveis locais podem ter o mesmo nome em outro escopo, apenas variáveis globais ou locais, no local que foi definido, não podem ter nomes iguais).
A variável pode assumir um papel de ação, quando o valor inicial é modificado ao longo da execução de um programa, ou papel de controle, quando seu valor é “vigiado” e utilizado em operações lógicas de decisão e laços de repetição ao longo de um programa. Ou seja, uma variável é a representação de uma região de memória utilizada para armazenar, acessar e modificar certo valor por um determinado espaço de tempo. 
*/Uma boa prática é escolher nomes significativos para as variáveis, ajudando a tornar um programa auto-explicativo/*
*/O C faz distinção entre letras maiúsculas e minúsculas (case sensitive, sensível a caixa alta/baixa) e por isso a1 e A1 são identificadores diferentes.
 Identificadores que começam com uma letra maiúscula serão atribuídos a um significado especial, que será visto posteriormente. /*
Algoritmos [Cap.3]
Inteiro: Números pertencentes ao conjunto de números inteiros, sem casas decimais (ex: 10, -5). O tipo de dado inteiro é utilizado em operações de processamento matemático. 
Em português estruturado, a representação do dado inteiro é feita com o comando INTEIRO.
Real: Números pertencentes ao conjunto de números reais, com casas decimais, fracionários e inteiros (ex: 4.50, 3.14).
Em português estruturado, representado pelo comando REAL. O tipo de dado real é utilizado em operações de processamento matemático.
Caractere / Cadeia: Textos ou letras soltas, delimitados por aspas (ex: "Curso", "A"). Também podem ser números (de 0 até 9) e símbolos impressos existentes em um teclado.
Representado em português estruturado pelos comandos CARACTERE ou CADEIA. Os tipos de dados caractere  ou cadeia são normalmente utilizados em operações de entrada e saída de dados. Caractere faz referência a um único caractere, já o cadeia quando é um conjunto de caracteres.
Lógico: Valores binários do tipo sim e não, verdadeiro ou falso, 1 e 0.
Representado em português estruturado pelo comando LÓGICO. Utilizado em operações de processamento lógico através das formas dos valores .F.(ou .FALSO.) e V(ou .VERDADEIRO.). Também podem ser utilizados os valores .S.(ou .SIM.) e .N.(ou .NÃO.).
C [Cap.3] 
O C exige que você declare o tamanho e o tipo da variável antes de colocar qualquer coisa dentro dela. Se tentar colocar um texto numa variável declarada como número, o programa gera um erro na compilação.
int (Inteiro)
Ao coletar o dado, como em um scanf, usa-se a abreviação d, com o operador de sequência de escape, %d.
float ou double (Real)
	Ao coletar o dado, como em um scanf, usa-se a abreviação f para float, com o operador de sequência de escape, %f, e lf para double, com o operador %lf.
char (Caractere) e String
Ao coletar o dado, como em um scanf, usa-se a abreviação c, com o operador de sequência de escape, %c. Em strings utilizamos o s, ficando com o operador %s.
bool (booleano)
Python [Cap. ] 
	Em Python você não precisa declarar o tipo da variável antes de usá-la. No momento em que você guarda um valor, o interpretador descobre automaticamente o tipo da variável e aloca o espaço na memória.
*/Se não tiver certeza sobre qual é o tipo de certo valor, o interpretador pode dizer isso a você:
>>> type(‘Hello’)
class ‘str’(string)/*
*/Se os números estiverem entre aspas, o python os considerará strings. Eles também não podem ser separados por vírgula, mas deve-se utilizar pontos./*
int (Inteiro)
float (Real)
str (String/Texto)
bool (Lógico/Booleano)
Diferenças C e Py: Em C, a tipagem é estática (int, chat, float). Em Python, a tipagem é dinâmica, o que significa que não é necessário declarar o tipo; a linguagem descobre pelo valor que você atribui.
Constantes [Algoritmos Cap.3]
	Constante é tudo o que é fixo, estável, inalterável, imutável, contínuo, de valor fixo e que é aplicado em diversos pontos de vista. Do ponto de vista computacional, que é semelhante ao matemático ou científico, constante é uma grandeza numérica fixa utilizada normalmente em uma expressão aritmética ou lógica, a qual define um valor que será inalterado na expressão, independentemente das variáveis envolvidas na operação a ser realizada. 
	Computacionalmente, ela pode ser classificada de três formas: implícita (quando definida dentro da linguagem com rótulos a serem utilizados nas operações de processamento), explícitas (quando definidas dentro do código pelo próprio desenvolvedor para uso do programa em uso) e internas (quando é parte da composição das equações matemáticas).
	As constantes seguem as mesmas regras de definição de nomes que as variáveis.
	Como exemplo prático, declararemos a constante matemática pi e uma expressão matemática em Português estruturado.

Português estruturado [Manzano Cap. 3]
 
SAIDA = ENTRADA + 1.23    //1.23 é a constante
ou
PI = 3.14159265
SAIDA = ENTRADA + PI //PI é a constante

Em C, basta atribuir o valor requerido a constante na sua declaração, já em python não tem como declarar uma constante pois não tem bloqueador nativo.	
Operadores Aritméticos
	Os operadores Aritméticos são responsáveis pelas operações matemáticas a serem realizadas em um computador. O termo operador é utilizado na área de programação para estabelecer as ferramentas responsáveis por executar algum tipo de ação computacional. Os operadores aritméticos são responsáveis pela execução do processamento matemático, exceto o operador de atribuição, que pode ser usado também em ações de processamento lógico. Eles são classificados em duas categorias, binários e unários. São binários quando utilizados em operações matemáticas de radiciação, exponenciação, divisão, multiplicação, adição e subtração; são unários quando atuam na inversão do estado de um valor numérico que pode ser passado de positivo para negativo ou vice-versa. 
Chaves e colchetes são abolidos, utilizando em seu lugar apenas os parênteses. [Manzano, Cap.3.5]
//As regras e precedência de operadores são as mesmas utilizadas em álgebra. Veja mais no Capítulo 2.5 de “Como programar em C” ou no Capítulo 2.5 de “Pense em Python”.
Algoritmos [Cap. 3]
	
	As tabelas abaixo apresentam os operadores segundo a ordem de prioridade matemática em que as operações são realizadas.O símbolo seta apontada para cima é a forma oficial de representação da operação de exponenciação para a indicação de cálculos de potências e raízes apresentado por Backus et al.*

	As expressões Aritméticas, operação comum para o estabelecimento de processamentos matemáticos, são realizadas a partir do relacionamento existente entre variáveis e constantes numéricas com a utilização dos operadores aritméticos. 
	O sinal de atribuição matemática, identificado pelo símbolo (=), é substituído pela seta para a esquerda, indicando a operação de atribuição. No exemplo de calcular a área de uma circunferência, escreveríamos como:
	AREA ← 3.14159265 * RAIO ↑  2
Outros exemplos:



Viraria -> A ← (B * H) / 2 



Viraria -> DELTA ← B ↑ 2 - 4 * A * C 
X1 ← (- B + DELTA ↑ ( 1 / 2 ) ) / ( 2 * A ) 
X2 ← (- B - DELTA ↑ ( 1 / 2 ) ) / ( 2 * A )
  





*/As variáveis X1 e X2 são utilizadas para representar, respectivamente, suas equivalentes matemáticas x’ e x’’. A variável DELTA representa sua equivalente matemática Δ. A definição de DELTA (½) representa a extração da raiz quadrada DELTA./*

C [Cap. 2] e Python [Cap.1.4 e 2.5]
	
	Alguns símbolos especiais não utilizados em álgebra estão presentes nas operações em C, como o asterisco (*), indicando multiplicação e o sinal de porcentagem (%), indicando o operador resto (modulus). 


	Para multiplicar a por b em álgebra, basta colocá-los lado a lado. Entretanto, se fizermos isto nesta linguagem, ab seria interpretado como um único nome (ou identificador) constituído de duas letras.
	A divisão inteira leva a um resultado inteiro, adquirindo o resto, se necessário, através do operador %, que só pode ser usado com operandos inteiros.

Python	
Python é bem semelhante à linguagem C ao abordar os operadores aritméticos, mas cabe adicionar o operador (**), que executa a exponenciação; isto é, eleva um número a uma potência, como:
>>> 6 ** 2 + 6
42 
	
*/A divisão por zero é impossível e quando não definida em sistemas computacionais resulta em um erro fatal, que faz com que o programa seja encerrado sem sucesso na realização de sua tarefa./*

*/Em C: Se você dividir dois números inteiros (ex: 5 / 2), o C joga fora as casas decimais e o resultado será 2. Para dar 2.5, as variáveis precisam ser float.
Em Python 3: O interpretador é mais moderno. Se você fizer 5 / 2, ele automaticamente devolve um float 2.5. Se você quiser que o Python jogue os decimais fora igual ao C, deve usar a divisão inteira com duas barras: 5 // 2./*
Lendo códigos simples e somando dois números inteiros
*/	Um prompt diz ao usuário para realizar uma ação específica, como: 
printf(“Digite um número\n”);/*

Diagrama de blocos








Português Estruturado

INICIO
INTEIRO: inteiro1, inteiro2, soma 
ESCREVA("Entre com o primeiro inteiro") 
LEIA(inteiro1) 
ESCREVA("Entre com o segundo inteiro") 
LEIA(inteiro2) 
soma <- inteiro1 + inteiro2 
ESCREVA("A soma e ", soma) 
FIM 


C [Cap.2]
	

O comentário indica o objetivo do programa, a linha que inclui a biblioteca (#include <stdio.h>) é uma diretiva para o pré-processador C e diz ao compilador para incluir no programa o arquivo padrão de entrada/saída. As linhas que começam com # são processadas antes de o programa ser compilado. Esta linha em particular diz ao pré-processador para incluir o conteúdo do arquivo de cabeçalho de entrada/saída padrão (standard input/output headerfile, stdio.h).
	A execução de todos os programas começa com main. A chave esquerda { marca o início do corpo de main e a chave direita marca o fim de main.
	A linha 4 é uma declaração, e as expressões inteiro1, inteiro2 e soma são os nomes das variáveis, do tipo int, inteiro. Muitas variáveis do mesmo tipo podem estar presentes em uma declaração. As declarações devem ser colocadas depois das chaves e antes de qualquer instrução executável, para não causar erros de sintaxe/erros de compilação.
	A função scanf recebe a entrada do dispositivo padrão. A da linha 6 tem dois argumentos “%d e &inteiro”. O segundo argumento começa com um e-comercial(&, ampersand, em inglês) - chamado em C de operador de endereço - seguido do nome da variável, dizendo ao scanf o local na memória onde a variável inteiro1 está armazenada. O computador então armazena o valor de inteiro1 naquele local.
*/Por parecer um diálogo a interação entre o prompt do printf e o valor recebido do scanf, essa interação é chamada frequentemente de computação conversacional ou computação interativa./* 
O /n é uma sequência de escape e posiciona o cursor no início da próxima linha.
A linha 9 contém uma instrução de atribuição. Ela calcula o valor da soma das variáveis inteiro1 e inteiro2 (através do operador +) e atribui o resultado à variável soma usando o operador de atribuição =.
A instrução “return 0;” passa o valor 0 de volta para o ambiente do sistema operacional no qual o programa está sendo executado. Isto indica para o sistema operacional que o programa foi executado satisfatoriamente.	 
//Mais detalhes e explicações das linhas no capítulo correspondente. 

Dicas em casos de erro: Verifique se o e-comercial está precedendo a variável na instrução scanf; confira se está fechando os blocos de instruções com ponto-e-vírgula; verifique se o % está presente e correto, com o tipo certo; não utilize o e-comercial em uma instrução printf se for iniciante e o código for simples.

Python
inteiro1 = int(input("Entre com o primeiro inteiro\n")) 
inteiro2 = int(input("Entre com o segundo inteiro\n")) 
soma = inteiro1 + inteiro2 
print(f"A soma e {soma}") 

Ler o código da direita para a esquerda em python facilita a leitura. O comando input() mostra a mensagem na tela e capta o que será digitado inicialmente como string(texto). Depois, ele pega o texto digitado e converte para um número inteiro (comando int(...)). 
O valor numérico convertido é atribuído à variável inteiro1, e o mesmo acontece com a variável inteiro2. 
A variável soma recebe estes inteiros e realiza a operação de soma, que está sendo solicitada através do operador aritmético (+).
Por fim, uma mensagem é mostrada na tela através de um print. O f significa format(formatação). Em Python, chamamos isso de f-string (Formatted String) e serve para mostrar que é necessário buscar o dado que será colocado na chave que mostra o conteúdo da variável soma, {soma}. Sem o f tudo é impresso como texto e as chaves também são mostradas.
*/A formatação com f-strings (print(f"Texto {variavel}")) é a forma mais moderna e recomendada, mas só funciona do Python 3.6 em diante. Se rodar em um ambiente mais antigo, vai gerar um SyntaxError. Nesses casos de emergência, use o .format(). /*
Python [Cap. 2]

	Uma instrução de atribuição cria uma nova variável e dá um valor a ela:
>>> message = ‘And now for’
>>> n = 17
>>> pi = 3.1415
Esse exemplo faz três atribuições. A primeira atribui uma string a uma nova variável chamada message; a segunda dá o número inteiro 17 a n; a terceira atribui o valor (aproximado) de pi a pi. 

Lendo código simples com strings

Em geral, não é possível executar operações matemáticas com strings, mesmo se elas parecerem números, então coisas assim são ilegais:
>>> ‘2’ - ‘1’
>>> ‘eggs/’easy’
Mas, em python, há duas exceções. O operador (+) executa uma concatenação de strings, ou seja, une as strings pelas extremidades. Por exemplo:
>>> first = ‘throat’
>>> second = ‘warbler’
>>> first + second
throatwarbler

O operador * também funciona em strings; ele executa a repetição com o número determinado. Por exemplo, “Spam” * 3 é igual aa “SpamSpamSpam. Neste caso, um dos valores precisa ser uma string e outro tem de ser um número inteiro.
Conceitos sobre Memória [Deitel Cap. 2]
Nomes de variáveis como inteiro1, inteiro2 e soma correspondem realmente a locais na memória do computador. Todas as variáveis possuem um nome, um tipo e um valor. Quando a instrução - Uma instrução é uma unidade de código que tem um efeito, como criar uma variável ou exibir um valor. [Downey Cap.2.3] - “scanf(“%d”, &inteiro1);” é executada, o valor digitado pelo usuário é colocado no local da memória ao qual o nome inteiro1 foi atribuído. Supondo que o valor digitado pelo usuário tenha sido 45, o computador colocará 45 no local inteiro1. E sempre que um valor é colocado em um local da memória, o novo valor invalida o anterior naquele local, pois as informações anteriores são destruídas. O processo de levar (ler) as informações para um local da memória C é chamado leitura destrutiva (destructive read-in). Considerando os valores da soma de dois inteiros anteriormente apresentados, quando a soma de inteiro1 e inteiro2 acontece eles ficam exatamente como antes de serem usados no cálculo da soma. Esses valores foram usados, mas não destruídos, quando o computador realizou o cálculo. Dessa forma, quando um valor é lido em um local da memória, o processo é chamado leitura não destrutiva.

Operadores Relacionais 
 As instruções executáveis realizam ações (como cálculos ou entrada e saída de dados) ou tomam decisões. Podemos, por exemplo, determinar se a nota de uma pessoa é maior ou igual a 60 e, se for, imprimir a mensagem “Parabéns! Você passou.” Os operadores relacionais são usados para testar condições (geralmente dentro de um if). "Fazendo uma pergunta" à CPU, e a resposta é sempre Verdadeiro ou Falso.

	Os operadores de igualdade possuem nível de precedência menor do que o dos operadores relacionais.
	Esta figura é dos operadores relacionais em C, mas mudam minimamente em Python e Algoritmos.
Diferente: Usa-se != (Em pseudocódigo usa-se <>).
Igualdade: Usa-se == (dois sinais de igual).
Confundir o operador de atribuição com o de comparação é um erro comum. Lembre-se: Um único sinal de igual (=) significa atribuição (Ex: idade = 20). Dois sinais de igual (==) significa comparação (Ex: if (idade == 20)).
Para evitar essa confusão, o operador de igualdade (==) deve ser lido como “é igual a” e o operador de atribuição (=) deve ser lido como “obtém” (ou recebe).
Sequências de Escape [Deitel Cap. 2]
Quando queremos que o texto impresso no ecrã tenha uma formatação visual específica – como uma quebra de linha ou um espaçamento longo –, utilizamos as sequências de escape. 



PRINCIPAIS DIFERENÇAS ENTRE C E PYTHON, NA ESCRITA DOS CÓDIGOS
Comandos de Entrada e Saída: Em C, precisamos de comandos separados para exibir uma mensagem (printf) e para capturar dados (scanf). Em Python, o comando input() faz ambas as coisas simultaneamente. Para saída simples, Python usa apenas print.
Declaração e Tipos (Tipagem): Em C, toda variável precisa ter seu tipo (int, float, char) declarado antes de ser usada. O Python é dinâmico e cria a variável no momento em que você a usa. Porém, atenção: tudo o que o usuário digita via input() em Python entra como texto (string). Para fazer contas matemáticas com o que foi digitado, é necessário converter explicitamente esse texto para número usando comandos como int() ou float(). 
Uso de Aspas: Em C, a regra é rígida: aspas simples (' ') são exclusivas para um único caractere e aspas duplas (" ") para cadeias de texto. Em Python, não há distinção; ambas podem ser usadas livremente para criar strings de qualquer tamanho. 

































SUMÁRIO DESTA PARTE
EXERCÍCIOS DE REVISÃO 1.1 [Deitel]	1
1.2 Preencha as lacunas em cada uma das sentenças a seguir sobre o ambiente C.	2
RESPOSTAS	2
EXERCÍCIOS CAP.1 [Downey]	3
EXERCÍCIOS ALGORITMOS CAP. 3 (EM DIAGRAMA, PY. E C)	4
SOMANDO DOIS INTEIROS	4
CÁLCULO DA ÁREA DE UM CÍRCULO	4
CÁLCULO DO SALÁRIO DE UM PROFESSOR	5


EXERCÍCIOS DE REVISÃO 1.1 [Deitel]
Preencha as lacunas em cada uma das sentenças a seguir. 
a) A companhia que criou o fenômeno da computação pessoal foi _______________. 
b) O computador que validou o uso da computação pessoal no comércio e na indústria foi o _______________. 
c) Os computadores processam dados sob o controle de um conjunto de instruções chamados_______________. 
d) As seis unidades lógicas do computador são_______________, _______________, _______________,_______________,_______________ e _______________. 
e) _______________ é um caso especial de multiprogramação na qual os usuários têm acesso ao computador através de dispositivos chamados terminais. 
f). As três classes de linguagens analisadas neste capítulo são_______________ , ____________ e _______________. 
g) Os programas que traduzem os programas em linguagem de alto nível para linguagem de máquina são chamados _______________. 
h) O C é muito conhecido como a linguagem de desenvolvimento do sistema operacional _______________. 
i) Este livro apresenta a versão do C chamada _______________ C, que foi padronizada recentemente pelo American National Standards Institute. 
j) A linguagem _______________ foi desenvolvida por Wirth para ensinar programação estruturada nas universidades. 
k) O Departamento de Defesa dos Estados Unidos (DOD) desenvolveu a linguagem Ada com um recurso chamado _______________ que permite aos programadores especificarem muitas atividades para serem executadas em paralelo. 
1.2 Preencha as lacunas em cada uma das sentenças a seguir sobre o ambiente C. 
a) Os programas em C são digitados normalmente em um computador usando um programa _______________. 
b) Em um sistema C, um programa _______________ é executado automaticamente antes de a fase de tradução começar. 
c) Os dois tipos mais comuns de diretivas de um pré-processador são _______________ e _______________. 
d) O programa _______________ combina a saída do compilador com várias funções da biblioteca para produzir uma imagem executável. 
e) O programa_______________ transfere a imagem executável do disco para a memória. 
f) Para carregar e executar o programa compilado mais recentemente em um sistema UNIX, digite _______________. 
RESPOSTAS
a) A companhia que criou o fenômeno da computação pessoal foi a Apple. 
b) O computador que validou o uso da computação pessoal no comércio e na indústria foi o IBM Personal Computer. 
c) Os computadores processam dados sob o controle de um conjunto de instruções chamados programas de computador. 
d) As seis unidades lógicas do computador são: Unidade de Entrada,Unidade de Saída,Unidade Lógica e Aritmética,Unidade de Memória,Unidade de Processamento Central e Unidade de Armazenamento Secundário. 
e) Timesharing é um caso especial de multiprogramação na qual os usuários têm acesso ao computador através de dispositivos chamados terminais. 
f) As três classes de linguagens analisadas neste capítulo são: Linguagens de Máquina, Linguagens Assembly e Linguagens de Alto Nível. 
g) Os programas que traduzem os programas em linguagem de alto nível para linguagem de máquina são chamados Compiladores. 
h) O C é muito conhecido como a linguagem de desenvolvimento do sistema operacional UNIX. 
i) Este livro apresenta a versão do C chamada ANSI C, que foi padronizada recentemente pelo American National Standards Institute. 
j) A linguagem Pascal foi desenvolvida por Wirth para ensinar programação estruturada nas universidades. 
k) O Departamento de Defesa dos Estados Unidos (DOD) desenvolveu a linguagem Ada com um recurso chamado Multitasking que permite aos programadores especificarem muitas atividades para serem executadas em paralelo. 
1.2 
a) Os programas em C são digitados normalmente em um computador usando um programa editor. 
b) Em um sistema C, um programa Pré-processador é executado automaticamente antes de a fase de tradução começar. 
c) Os dois tipos mais comuns de diretivas de um pré-processador são a inclusão de outros arquivos e a substituição de símbolos especiais por texto de programa. 
d) O programa linker(ligador) combina a saída do compilador com várias funções da biblioteca para produzir uma imagem executável. 
e) O programa carregador(loader) transfere a imagem executável do disco para a memória. 
f) Para carregar e executar o programa compilado mais recentemente em um sistema UNIX, digite a.out. 

EXERCÍCIOS CAP.1 [Downey]
1. Em uma instrução print, o que acontece se você omitir um dos parênteses ou ambos? 
2. Se estiver tentando imprimir uma string, o que acontece se omitir uma das aspas ou ambas? 
3. Você pode usar um sinal de menos para fazer um número negativo como -2. O que acontece se puser um sinal de mais antes de um número? E se escrever assim: 2++2? 
4. Na notação matemática, zeros à esquerda são aceitáveis, como em 02. O que acontece se você tentar usar isso no Python? 
5. O que acontece se você tiver dois valores sem nenhum operador entre eles?

 Inicialize o interpretador do Python e use-o como uma calculadora. 
1. Quantos segundos há em 42 minutos e 42 segundos? 
2. Quantas milhas há em 10 quilômetros? Dica: uma milha equivale a 1,61 quilômetro. 
3. Se você correr 10 quilômetros em 42 minutos e 42 segundos, qual é o seu passo médio (tempo por milha em minutos e segundos)? Qual é a sua velocidade média em milhas por hora? 

EXERCÍCIOS ALGORITMOS CAP. 3 (TAMBÉM APLICADOS EM PYTHON E C)
SOMANDO DOIS INTEIROS
1 - Desenvolver um programa de computador que efetue a leitura de dois valores numéricos inteiros. Processe a operação de adição dos dois valores e apresente na sequência a soma obtida com a operação.
Fiz isso na parte de arquitetura, tipos de dados e sintaxe
CÁLCULO DA ÁREA DE UM CÍRCULO 
2 - Elaborar um programa de computador que calcule a área de uma circunferência e apresentar a medida da área calculada

Descrição das etapas de entendimento do problema:
1. Estabelecer que pi venha a possuir o valor 3.14 
2. Ler um valor para o raio.
3. Efetuar o cálculo da área, elevando ao quadrado o valor de raio e multiplicando esse valor por pi.
4. Apresentar o valor da variável A (área).

 A área de uma circunferência é calculada multiplicando a constante pi (aproximadamente (3,14) pelo quadrado do raio.
  Então, A = pi * raio^2
 
Diagrama de blocos:


Codificação:
programa AREA_CIRCULO
const
		pi = 3.14
var
		A : real
		raio : real
início
		leia raio
		a <- pi * (raio * raio)
		escreva A
fim



C:

#include <stdio.h>

int main() {
    float pi = 3.14159265;
    float raio, A;
    printf("Digite o raio da circunferencia\n");
    scanf("%f", &raio);
    A = pi * (raio * raio);
    printf("A area da circunferencia e %.2f\n", A);
    return 0;
}

python:

pi = 3.14159265
raio = float(input("Digite o raio da circunferencia\n"))
A = pi * (raio * raio)
print(f"A area da circunferencia e {A:.2f}")
CÁLCULO DO SALÁRIO DE UM PROFESSOR
3 - Desenvolver um programa que calcule o salário líquido de um professor. Para elaborar o programa, é necessário possuir alguns dados, como valor da hora-aula, número de horas trabalhadas no mês e percentual de desconto do INSS. Em primeiro lugar, deve-se estabelecer o seu salário bruto para fazer o desconto e ter o valor do salário líquido.
Ler os valores de HA (Hora-aula), HT (horas trabalhadas) e PD (percentual de desconto).
O salário bruto (SB) é calculado a partir do valor da hora-aula (HA) vezes o número de horas trabalhadas (HT).
Os descontos são considerados como o PD * SB
O salário líquido (SL) será calculado a partir do salário bruto (SB) - descontos.
Mostrar os valores de SB e SL.

Diagrama de blocos:

C:
#include <stdio.h>

int main() {
    double HA, HT, PD, descontos, SB, SL;
    printf("Insira os valores referentes a hora-aula, horas trabalhadas (mensal) e percentual de desconto(em decimal)\n");
    scanf("%lf %lf %lf", &HA, &HT, &PD);
    SB = HA * HT;
    descontos = PD * SB;
    SL = SB - descontos;
    printf("Salario bruto: %.2lf\n Salario liquido: %.2lf", SB, SL);
    return 0;
}

python:

HA = float(input("Digite o valor da sua hora-aula\n"))
HT = float(input("Digite sua hora trabalhada mensal\n"))
PD = float(input("Digite o percentual de desconto em decimal\n"))
SB = HA * HT
Descontos = SB * PD
SL = SB - Descontos
print(f"Salario Bruto {SB}\nSalario Liquido {SL}\n")

NOME E SEXO
4 - Desenvolver um programa que faça a entrada do nome de uma pessoa e de seu sexo. Em seguida, apresentar os dados anteriormente informados.
Ler nome e sexo.
Mostrar nome e sexo.

Diagrama de blocos:



C:
#include <stdio.h>

int main() {
    char NOME[30]; 
    char SEXO;
    printf("Qual é o seu nome?\n");
    scanf("%s", &NOME);
    printf("Qual é o seu sexo (M ou F)?\n");
    scanf(" %c", &SEXO);
    printf("%s, %c", NOME, SEXO);
    return 0;
}

python:


NOME = input("Escreva o seu nome\n")
SEXO = input("Qual é o seu sexo? (M ou F)\n")
print(NOME, SEXO)

EXERCÍCIOS DE FIXAÇÃO
1. Escreva ao lado de cada valor o tipo em que se enquadra (inteiro, real, caractere, cadeia ou lógico), levando em consideração que um valor numérico pertencente ao conjunto de valores numéricos inteiros está contido também no conjunto de valores numéricos reais.
-456 _______________        .F. _______________ 
.Falso. ______________      .V. _______________
 “0.87” _______________     “0” _______________ 
“-9.12” _______________     “-900” _______________ 
“Casa 8” _______________  “Cinco” _______________ 
“V” _______________           0 _______________ 
1.56 _______________         -1.56 _______________ 
34 _______________            45.8976 ___________
-465 _______________         678 _______________
-678 _______________         -99.8 _______________ 
“.V.” _______________          1000 ______________  

2. Assinale com um X os nomes válidos para uma variável

(  ) ENDEREÇO                     (  ) END*A-6
(  ) 21BRASIL                        (  ) CIDADE3
(  ) FONE$COM                     (  ) #CABEC
(  ) NAMEUSER                     (  ) REAL
(  ) NOME_USUÁRIO            (  ) REAL$
(  ) NOME*USUÁRIO             (  ) SOBRENOME

3. Dada as equações matemáticas a seguir, estabeleça para cada uma delas a respectiva expressão aritmética em estilo computacional.








4. Desenvolver os diagramas de bloco e a codificação em português estruturado dos problemas computacionais elencados de a até z.
Por ser extenso e muito básico, pularemos alguns destes exercícios. 

a) Ler uma temperatura em graus Celsius e apresentá-la convertida em graus Fahrenheit. A fórmula de conversão é F ← C * 9 / 5 + 32, sendo F a temperatura em Fahrenheit e C a temperatura em Celsius.

c) Calcular e apresentar o valor do volume de uma lata de óleo, utilizando a fórmula VOLUME ← 3.14159 * R ↑ 2 * ALTURA 

r) Em uma eleição sindical concorreram ao cargo de presidente três candidatos (representados pelas variáveis A, B e C). Durante a apuração dos votos foram computados votos nulos e em branco, além dos votos válidos para cada candidato. Deve ser criado um programa de computador que faça a leitura da quantidade de votos válidos para cada candidato, além de ler também a quantidade de votos nulos e em branco. Ao final, o programa deve apresentar o número total de eleitores, considerando votos válidos, nulos e em branco; o percentual correspondente de votos válidos em relação à quantidade de eleitores; o percentual correspondente de votos válidos do candidato A em relação à quantidade de eleitores; o percentual correspondente de votos válidos do candidato B em relação à quantidade de eleitores; o percentual correspondente de votos válidos do candidato C em relação à quantidade de eleitores; o percentual correspondente de votos nulos em relação à quantidade de eleitores; e, por último, o percentual correspondente de votos em branco em relação à quantidade de eleitores. Todos os cálculos devem efetivamente ser armazenados em memória. 
RESPOSTAS DOS EXERCÍCIOS
1 - 
-456 _inteiro e real          .F.  lógico  
.Falso.  lógico                  .V.  lógico 
 “0.87” cadeia                  “0” caractere ou cadeia   
“-9.12” cadeia                  “-900” cadeia 
“Casa 8” cadeia               “Cinco” cadeia 
“V” caractere                    0 inteiro e real
1.56 real                          -1.56 real 
34 inteiro e real                45.8976 real
-465 inteiro e real             678 inteiro e real
-678 inteiro e real            -99.8 real 
“.V.” cadeia                      1000 inteiro e real 

2 - 
(  ) ENDEREÇO                     (  ) END*A-6
(  ) 21BRASIL                        (X) CIDADE3
(  ) FONE$COM                     (  ) #CABEC
(X) NAMEUSER                     (  ) REAL
(X) NOME_USUÁRIO            (  ) REAL$
(  ) NOME*USUÁRIO             (X) SOBRENOME

3 - 
f ← ((1 / 1 * c)) - (r ↑ 2 / 4 * c ↑ 2)) ↑ (1 / 2)

X ← a / (b - c)

X ← m * (a * h + v ↑ 2 / 2)

d ← v * t + a * t ↑ 2 / 2

d ← (p - r) / n

f ← c * 9 / 5 + 32

c ← (f - 32) * 5 / 9























*Símbolos normalizados - ISO 5807

//Para mais informações sobre como utilizar os símbolos veja o livro do Manzano, capítulo 2.3.2









Palavras-chave em Python


Palavras-chave em C


Palavras-chave em Português estruturado:
ATÉ, ATÉ_QUE, ATÉ_SEJA, CADEIA, CARACTERE, CASO, CLASSE, CONJUNTO, CONST, CONTINUA, DE, EFETUE, ENQUANTO, ENQUANTO_SEJA, ENTÃO, ESCREVA, FAÇA, FIM, FIM_ATÉ_SEJA, FIM_CASO, FIM_CLASSE, FIM_ENQUANTO, FIM_FAÇA, FIM_LAÇO, FIM_PARA, FIM_REGISTRO, FIM_SE, FUNÇÃO, HERANÇA, INÍCIO, INTEIRO, LAÇO, LEIA, LÓGICO, PARA, PASSO, PRIVADA, PROCEDIMENTO, PROGRAMA, PROTEGIDA, PÚBLICA, REAL, REGISTRO, REPITA, SAIA_CASO, SE, SEÇÃO_PRIVADA, SEÇÃO_PROTEGIDA, SEÇÃO_PÚBLICA, SEJA, SENÃO, TIPO, VAR e VIRTUAL 









RESUMO
• É o software (i.e., as instruções que você escreve para ordenar ao computador a realização de ações e a tomada de decisões) que controla os computadores (chamados freqüentemente de hardware). 
• ANSI C é a versão da linguagem de programação C padronizada em 1989 tanto nos Estados Unidos, através do American National Standards Institute (ANSI), como em todo o mundo, através da International Standards Organization (ISO).
 • Os computadores que podem ter ocupado salas enormes e custado milhões de dólares há 25 anos podem agora estar contidos na superfície de chips de silício menores do que uma unha e que talvez custem alguns dólares cada um. 
• Aproximadamente 150 milhões de computadores de uso geral estão em atividade em todo o mundo, ajudando as pessoas nos negócios, indústria, governo e em suas vidas pessoais. Este número pode dobrar facilmente em alguns anos.
 • Um computador é um dispositivo capaz de realizar cálculos e tomar decisões lógicas com uma rapidez milhões, ou mesmo bilhões, de vezes maior do que os seres humanos.
 • Os computadores processam dados sob o controle de programas computacionais. 
• Os vários dispositivos (como teclado, tela, discos, memória e unidades de processamento) que constituem um sistema computacional são chamados de hardware.
 • Os programas executados em um computador são chamados de software. 
• A unidade de entrada é a seção de "recepção" do computador. Atualmente a maioria das informações é fornecida aos computadores através de teclados como os de máquinas de escrever. 
• A unidade de saída é a seção de "expedição" do computador. Atualmente, a maioria das informações é fornecida pelos computadores através de exibição na tela ou impressão em papel. 
• A unidade de memória é a seção de "armazenamento" do computador e é chamada frequentemente de memória, memória principal ou memória primária. 
• A unidade aritmética e lógica (arithmetic and logic unit, ALU) realiza os cálculos e toma decisões.
 • A unidade central de processamento, UCP (central processing unit) é a responsável pela coordenação do computador e pela supervisão do funcionamento de outras seções.
 • Normalmente, os programas ou dados que não estiverem sendo usados ativamente por outras unidades são colocados em dispositivos de armazenamento secundário (como discos) até que sejam novamente necessários. 
• No processamento de lotes de usuário único (single-user batch processing), o computador executa um programa simples de cada vez enquanto processa os dados em grupos ou lotes (batches).
• A multiprogramação envolve a realização "simultânea" de várias tarefas no computador — este compartilha seus recursos entre as tarefas.
 • Timesharing (tempo compartilhado) é um caso especial de multiprogramação na qual os usuários têm acesso ao computador por intermédio de terminais. Parece que os usuários estão executando programas simultaneamente. 
• Com a computação distribuída, o poder computacional de uma organização é distribuído através de uma rede para os locais (sites) nos quais o trabalho real da organização é realizado.
 • Os servidores de arquivo armazenam programas e dados que podem ser compartilhados por computadores clientes distribuídos ao longo da rede, daí o termo computação cliente/servidor. 
• Qualquer computador pode entender diretamente sua própria linguagem de máquina. 
• Geralmente, as linguagens de máquina consistem em strings de números (reduzidos em última análise a ls e Os) que mandam o computador realizar suas operações mais elementares, uma por vez. As linguagens de máquina dependem do equipamento.
 • Abreviações semelhantes ao idioma inglês formam a base das linguagens assembly. Os assemblers (montadores) traduzem os programas em linguagem assembly para linguagem de máquina.
 • Os compiladores traduzem os programas em linguagem de alto nível para linguagem de máquina. As linguagens de alto nível contêm palavras em inglês e notações matemáticas convencionais. 
• O C é conhecido como a linguagem de desenvolvimento do sistema operacional UNIX.
 • É possível escrever programas em C que sejam portáveis para a maioria dos computadores. 
• O padrão ANSI C foi aprovado em 1989. 
• O FORTRAN (FORmula TRANslator) é usado em aplicações matemáticas. 
• O COBOL (COmmon Business Oriented Language) é usado principalmente em aplicações comerciais que exijam manipulação precisa e eficiente de grandes volumes de dados. 
• Programação estruturada é um método disciplinado de escrever programas que sejam claros, visivelmente corretos e fáceis de serem modificados. 
• O Pascal destinava-se ao ensino de programação estruturada em ambientes acadêmicos. • A Ada foi desenvolvida sob o patrocínio do Departamento de Defesa dos Estados Unidos (United States" Department of Defense, DOD) usando o Pascal como base.
• A multitarefa (multitasking) da linguagem Ada permite aos programadores especificarem atividades paralelas. 
• Todos os sistemas em C consistem em três partes: o ambiente, a linguagem e as bibliotecas padrão. As funções da biblioteca não são parte da linguagem C em si; elas realizam operações como entrada/saída de dados e cálculos matemáticos. 
• Para serem executados, os programas em C passam geralmente por seis fases: edição, pré-processamento, compilação, linking (ligação), carregamento e execução.
 • O programador digita um programa com um editor e faz as correções necessárias.
 • Um compilador traduz um programa em C para linguagem de máquina (ou códigoobjeto). 
• Um pré-processador obedece a diretivas que indicam normalmente que outros arquivos devem ser incluídos no arquivo a ser compilado e que símbolos especiais devem ser substituídos por texto de programa.
 • Um linker liga o código-objeto ao código de funções que estejam faltando de modo a produzir uma imagem executável (com todas as partes necessárias).
 • Um loader (carregador) apanha uma imagem executável do disco e a transfere para a memória
. • Um computador, sob controle de sua CPU, executa, uma a uma, as instruções de um programa. 
• Determinadas funções do C (como scanf) recebem dados de stdin (o dispositivo padrão de entrada) que normalmente é atribuído ao teclado
. • Os dados são enviados a stdout (o dispositivo padrão de saída) que normalmente é a tela do computador.
 • Há ainda um dispositivo padrão de erro chamado stderr. O dispositivo stderr (normalmente a tela) é usado para exibir mensagens de erro. 
• Embora seja possível escrever programas portáteis, há muitos problemas entre as diferentes implementações do C e os diferentes computadores que podem fazer com que a portabilidade seja difícil de conseguir. 
• O Concurrent C é um superconjunto do C que inclui recursos para especificar a realização de várias atividades em paralelo.
 • O C++ fornece recursos para a realização de programação orientada a objetos.
 • Objetos são basicamente componentes reutilizáveis de software que modelam itens do mundo real.

Práticas Recomendáveis de Programação 
1.1 Escreva seus programas em C de uma maneira simples e objetiva. Algumas vezes isto é chamado KIS (do inglês "keep it simple" [que pode ser traduzido por "mantenha a simplicidade"]). Não "complique" a linguagem tentando soluções "estranhas". 1.2 Leia os manuais da versão do C que estiver usando. Consulte freqüentemente estes manuais para se certificar do conhecimento do rico conjunto de recursos do C e de que eles estão sendo usados corretamente. 1.3 Seu computador e compilador são bons mestres. Se você não estiver certo de como funciona um recurso do C, escreva um programa de teste que utilize esse recurso, compile e execute o programa, e veja o que acontece. Dicas de Portabilidade 1.1 Em face de o C ser uma linguagem independente de hardware e amplamente disponível, as aplicações escritas em C podem ser executadas com pouca ou nenhuma modificação em uma grande variedade de sistemas, computacionais. 1.2 Usar as funções da biblioteca padrão do C em vez de escrever suas próprias versões similares pode melhorar a portabilidade do programa porque estas funções estão colocadas em praticamente todas as implementações do ANSI C. 1.3 Embora seja possível escrever programas portáteis, há muitos problemas entre as diferentes implementações do C e os diferentes computadores que tornam a portabilidade um objetivo difícil de atingir. Simplesmente escrever programas em C não garante a portabilidade. Dica de Performance 1.1 Usar as funções da biblioteca padrão do C em vez de você escrever suas próprias versões similares pode melhorar o desempenho do programa porque essas funções foram desenvolvidas cuidadosamente por pessoal eficiente.

CAPÍTULO 1
1 Conceitos de Computação Objetivos  Entender os conceitos básicos do computador.  Familiarizar-se com os diferentes tipos de linguagens de programação.  Familiarizar-se com a história da linguagem de programação C.  Conhecer Biblioteca Padrão da linguagem C (C Standard Library).  Entender o ambiente e desenvolvimento de programas C.  Compreender por que é apropriado aprender C no primeiro curso de programação.  Compreender por que a linguagem C fornece uma base para estudos futuros de programação em geral e em particular para o C++. 
Sumário 1.1 1.2 1.3 1.4 Introdução O que É um Computador? Organização dos Computadores Processamento em Lotes (Batch Processing), Multiprogramação e Tempo Compartilha do (Timesharing) 1.5 Computação Pessoal, Computação Distribuída e Computação Cliente/Servidor 1.6 nível. 1.7 1.8 1.9 1.10 1.11 1.12 1.13 1.14 Linguagens de Máquina, Linguagens Assembly e Linguagens de Alto A História do C A Biblioteca Padrão (Standard Library) do C Outras Linguagens de Alto Nível Programação Estruturada Os Fundamentos do Ambiente C Observações Gerais sobre o C e Este Livro Concurrent C Programação Orientada a Objetos e C+ + 

CAPITULO 2
2 Introdução à Programação em C Objetivos • Ficar em condições de escrever programas computacionais simples em C. • Ficar em condições de usar instruções simples de entrada e saída. • Familiarizar-se com os tipos fundamentais de dados. • Entender os conceitos sobre a memória do computador. • Ficar em condições de usar os operadores aritméticos. • Entender a precedência de operadores aritméticos. • Ficar em condições de escrever instruções simples para tomada de decisões. 
Sumário 2.1 2.2 2.3 2.4 2.5 2.6 Introdução Um Programa Simples em C: Imprimir uma Linha de Texto Outro Programa Simples em C: Somar Dois Números Inteiros Conceitos sobre Memória Aritmética em C Tomada de Decisões: Operadores de Igualdade e Relacionais Resumo — Terminologia — Erros Comuns de Programação — Práticas Recomendáveis de Programação — Dica de Portabilidade — Exercícios de Revisão — Respostas dos Exercícios de Revisão — Exercícios 



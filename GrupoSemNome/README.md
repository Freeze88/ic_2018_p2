Computação1______________________________________

André Vitorino--a21802937
Joana Silva--a21805651


Solução e notas importantes______________________

No programa no ínicio foram colocadas as duas estruturas principais do programa, a primeira relativa ao jogador e os dados que este contêm, sendo fácil de acrescentar novos recursos.
Uma segunda é sobre o mapa, que regula toda a informação localizada no mapa, que, a qualquer momento também pode ser acrescentada ou mudada consoante o necessário.
Não exitem variáveis globais, e todas as outras são utilizadas o máximo de vezes possível para não gastar espaço em criar e alocar espaço para novas variáveis.

Fluxograma:
O fluxograma em termos pŕaticos é simples, apesar das funções criadas o program é muito linear na maneira como se executa.

Cria o mapa -> Guarda o mapa numa estrutura -> Pede ao jogador onde começar -> grava os dados numa outra estrutura -
-> Pede o que o jogador quer fazer -> caso tenha 6 pontos vê o vencedor -> pergunta se desejam jogar outra vez.

Uma vez que não é possível de enviar um duplo array para uma função vários ciclos "for" foram utilizados para contornar o problema e ainda mandar o array inteiro.


Manual___________________________________________

Para compilar o programa basta utilizar o ficheiro Makefile escrevendo "make" no terminal ou utilizar a combinação de comandos do GCC no programa "program.c".


_Regras_

No início do jogo, cada jogador escolhe um local para instalar a sua primeira aldeia (A). 

Em cada jogada, o jogador vai lançar dois dados. Todos os jogadores que tenham aldeias em posições com terrenos adjacentes cujo número for igual à soma dos dois dados, ganham um recurso natural produzidos pelos terrenos adjacentes.

Para expandir o seu território, cada jogador terá de colocar aldeias nos locais ligados a uma aldeia sua.


Cada posição só pode pertencer a um jogador e, se já estiver ocupada, este não pode ser escolhida.


Quando chega a sua vez, o jogador é lhe lançado os dados automáticamente e só depois pode fazer qualquer outra acção. Depois dos dados lançados enquanto tiver recursos para isso, o jogador pode:

--> Comprar uma aldeia e coloca-la numa posição adjacente;

--> Transformar uma aldeia (A) sua em uma cidade (C). Quando o jogador tem uma cidade, os terrenos adjacentes passam a produzir duas unidades de recurso natural em vez de uma;

--> Efectuar uma troca com o banco ao rácio 4 para 1. Para isso o jogador pode trocar 4 unidades iguais de um recurso natural, por uma carta de um recurso natural que necessite.

--> Efectuar uma troca com o banco: 
                                     -> 10 recursos em troca de um ponto;
                                     -> 4 recursos por 1 recurso á escolha.

--> Passar a vez ao outro jogador; 

--> O objectivo do jogo é chegar primeiro aos 6 pontos: 
                                     -> Cada aldeia vale 1 ponto;
                                     -> Cada cidade vale 2 pontos.

--> O jogo acaba quando um dos jogadores chegar aos 6 pontos.

--> Depois de um dos jogadores vencer é perguntado se quer jogar outra vez.

Preços:

-> Aldeia: B + L + G + W

-> Cidade: G + G + I + I + I

Conclusões_____________________________________


O projeto revelou-se maior que consegui-mos concretizar, coisas pedidas como a utilização do ficheiro "ini" foram testadas e tentadas várias vezes antes da realização do resto do código, no entanto devido a este não estar a resultar foi cortado a favor de focar em concretizar o resto do programa e deixar o "ini" como última preoridade.

O tempo para realizar o programa foi mal calculado, deixando pouco espaço para realizar extras ou incorporar o ficheiro "ini" mencionado anteriormente.

Alguma dificuldade em trabalhar em grupo, mas devido á pobre organização, com tarefas e a-fazer bem esclarecido, mas incorporação de código ser algo complicada devido a contrastes de criação do código. Por exemplo, um criou parte do programa em português enquanto outro utilizava inglês.

Ainda alguma dificuldade em utilizar o git, mas uma melhor percepção de ficheiros doxyfile e Makefile.


Referências____________________________________


O program foi feito inteiramente por nós próprios, com apenas procura de definições e/ou utilização de bibliotecas e palavras das quais não reconheciamos a sua utilidade.

Discusão com colegas sobre a utilização do ficheiro "ini" ao qual se conclui que apesar de existir o conhecimento de ter "FILE *fp" pouco mais conseguiam acrescentar.

Pergunta a um terceiro sobre a utilização de duplo array e como coloca-lo em funções.

Ajuda proveniente de um colega em particular que sugeriu que o input original scanf("%c",&input) fosse mudado para fgets(input, 128, stdin) e que as comparações seguintes utilizado o input utilizasem input[0], o que impedia de primir todas as teclas de uma vez.


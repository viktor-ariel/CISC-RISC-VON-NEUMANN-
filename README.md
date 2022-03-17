# CISC,RISC,VON NEUMANN 🧑‍💻

## Trabalho do curso em informática (pesquisa) 👨‍💻

### O que é CISC?
Cisc é uma arquitetura do computador. A arquitetura CISC, conhecida também como "Computador com um conjunto complexo de instruções" (Complex Instruction Set Computer), executa centenas de instruções complexas diferentes, sendo assim, extremamente versátil.

### O que é RISC?
Risc é uma arquitetura do computador.A arquitetura RISC, conhecida também como Computador com um conjunto reduzido de instruções (Reduced Instruction Set Computer), executa um conjunto simples e pequeno de instruções que levam aproximadamente a mesma quantidade de tempo para serem executadas.

### CISC vs RISC?
Considerado o cérebro de um computador, o processador – ou Unidade Central de Processamento (CPU) – é um circuito eletrônico responsável por executar uma série de instruções dadas pela máquina.   Essas instruções são pré-definidas e armazenadas na memória principal do computador e chegam ao processador em linguagem "assembly", que é o padrão reconhecido e compreendido por ele.   O processador pode receber diferentes tipos de instrução:

*Operações aritméticas (adição, subtração, multiplicação e divisão);
*Acesso à memória para, por exemplo, mover dados de um local para outro;
*Operações lógicas;
*Controle
*Etc...
É aqui que as diferenças entre RISC e CISC começam a surgir. CISC é o acrônimo de Complex Instruction Set Computer, ou seja, executa instruções complexas.

 E qual é a complexidade por trás dessas instruções?  

Elas são normalmente longas e repletas de operações matemáticas distintas.
Não possuem um tamanho padrão, podendo assumir dimensões variáveis de acordo com a quantidade de operações que deverão ser executadas.
Exigem que o processador acesse a memória para executar essa instrução.
Resultado: o tempo de processamento será maior afetando, portanto, a capacidade de processamento.  Para executar uma só instrução, um processador CISC pode exigir vários ciclos de relógio. Um ciclo de relógio é a frequência medida em Hertz que determina quantos impulsos serão realizados por segundo naquele computador.  

Exemplo, uma máquina de 100Mhz irá realizar 100 milhões de impulsos por segundo. Quanto maior esse número, menor será a quantidade de ciclos necessários para executar uma instrução.   A família de processadores x86 da Intel (286, 386, 486) nascida na década de 1970 é uma das mais reconhecidas usuárias da arquitetura CISC. E, durante anos, os computadores pessoais se restringiram a essa arquitetura até que a Apple mudou esse cenário.   “Podemos dizer que 90% do mercado têm suas demandas atendidas por máquinas com processador CISC. São usadas, normalmente, para rodar aplicações simples que exigem pouco processamento como um sistema de caixa de uma loja, por exemplo”, afirma o Diretor de Operações da LB2, Victor Machado.

 Devido à capacidade de processamento limitada, são logo substituídas pela arquitetura RISC, quando a necessidade de processamento atinge padrões elevados.

RISC ( Reduced Instruction Set Computer)
Aqui o nome mais uma vez diz muito sobre a arquitetura do processador. Ao contrário do CISC, o RISC executa instruções reduzidas. 

Ou seja, ele quebra a instrução em várias menores e mais simples e todas assumem um tamanho padrão.   Cada uma dessas instruções têm as características necessárias para que possa ser executada em apenas um ciclo de relógio. No exemplo que demos antes, a cada 100 milhões de impulsos, uma instrução seria concluída.

No caso do CISC, essa afirmação não seria verdadeira já que uma instrução poderia exigir 10, 20 ou vários outros ciclos para ser finalizada.   “Em nível enterprise, em que o processamento dos dados é muito alto, máquinas com arquitetura RISC como a Power da IBM e Sparc da Oracle são as mais indicadas. E aqui não estamos nos referindo necessariamente ao tamanho da empresa. Organizações de pequeno e médio porte podem ter operações que exijam capacidade de processamento muito alto e, por isso, recorrem ao RISC”, detalha Victor.  

O RISC também é amplamente utilizado em dispositivos móveis como celulares e tablets, os próprios notebooks e vídeo-games, pois são processadores menores, mais baratos e que tendem a consumir menos energia. Sem contar que atende à forte demanda por uma velocidade de processamento elevada nestes casos. 

### O que é cache?
A memória cache (a pronúncia correta é <b>“cash”</b>, e não “cachê”) é um tipo de memória que trabalha em conjunto com o processador. De fato, todos os processadores atuais trazem uma certa quantidade de memória cache embutida no encapsulamento. O objetivo é potencializar o desempenho do chip de processamento, evitando que fique ocioso por longos períodos.
A CPU (Central Processing Unit) trabalha diretamente com a memória RAM. Assim, todos os dados processados pelo chip são enviados pelos módulos de memória RAM.
<b>Acontece que a memória RAM é muito mais lenta do que o processador.</b> Em outras palavras, ele processa dados mais rápido do que a memória RAM pode enviar. Isso resulta em longos períodos de ociosidade e, consequentemente, desperdício de capacidade do processador.
<b>Para resolver esse problema e fazer com que a CPU trabalhe com a força máxima possível, foi criada a memória cache.</b> Ela é muito mais rápida que a memória RAM e tem a função de fornecer as informações mais cruciais para o processador.
<br>
Como funciona a memória cache?

Como visto, esse tipo de memória possui alta velocidade e tem por função armazenar dados e instruções que a CPU poderá precisar em breve. Ela possibilita que o processador trabalhe com toda a capacidade e tenha o mínimo de tempo ocioso possível.Cada fabricante utiliza a memória cache de uma forma diferente. Isso também pode variar de acordo com a microarquitetura usada no chip. No entanto, o padrão é que, quando a CPU precisa buscar a sua primeira instrução, ela terá de ir até a memória RAM, visto que a memória cache estará vazia. Apesar disso, em vez de trazer apenas a solicitação feita pela CPU, a unidade de busca traz um bloco inteiro de instruções que, por sua vez, é armazenado na memória cache. Assim, se o processador for continuar a executar o referido programa, as instruções subsequentes estarão já armazenadas na memória cache. Então, a unidade de busca não precisará ir até a memória RAM para obtê-las.
<br>
Níveis de memória cache
A memória cache é dividida em alguns níveis, conhecidos como L1, L2 e L3 (L significa Level, em inglês). Eles dizem respeito à proximidade da memória cache das unidades de execução do processador. Quanto mais próxima ela estiver da unidade de execução do processador, menor será o seu número. Assim, o cache L1 é o mais próximo possível. O L2 é um pouco mais distante e o L3 é ainda mais distante. Sempre que a unidade de busca do processador precisa de um novo dado ou instrução, ela procura inicialmente no cache L1. Se não encontrar, parte para o L2 e depois para o L3. Se a informação não estiver em nenhum dos níveis de memória cache, ela terá de ir até a memória RAM.
Uma peculiaridade a respeito dos níveis, é que o L1 é dividido em memória de instrução e memória para dados. Com isso, o processador vai direto à memória de instrução, se estiver buscando uma instrução, ou vai direto à memória de dados, se estiver buscando um dado. Isso agiliza ainda mais o processador de busca.
<br>

### Arquitetura de VON NEUMANN
A Arquitetura de computador de von Neumann<b> se caracteriza pela possibilidade de uma máquina digital armazenar seus programas no mesmo espaço de memória que os dados,</b> podendo assim manipular tais programas. Esta arquitetura é um projeto modelo de um computador digital de programa armazenado que utiliza uma unidade de processamento (CPU) e uma de armazenamento ("memória") para comportar, respectivamente, instruções e dados.

### Organizações das memórias
![image](https://user-images.githubusercontent.com/98894099/158712583-991647ed-325b-4a45-80cc-84029c653219.png)

Hierarquia de Memória (2)
 A memória cache é geralmente controlada por hardware
 A memória principal (RAM) e a secundária é que o usuário
tem acesso.
 O sistema operacional através de um mecanismo de
Memória Virtual (Segmentação e/ou Paginação) cria
a “ilusão” ao usuário que a memória total é do tamanho da memória principal + memória secundária.
 A técnica de memória virtual realiza transferência de blocos
de informação entre a memória primária e secundária automaticamente sem a intervenção do usuário comum.

Registradores
 São dispositivos (elementos computacionais)
capazes de receber dados, mantê-los armazenados
por uma curto período de tempo e transferi-los
para outro dispositivo.
 São, portanto, elementos de armazenamento
temporário.
 Os registradores fazem parte da CPU.
 São extremamente rápidos e armazenam grupos
reduzidos de bits.
<br><br><br>
Memória Principal 
 A memória é a parte do computador em que os programas e os dados são armazenados.
 A memória principal (MP) armazena programas em execução e os dados utilizados por eles.
 Sem uma memória na qual processadores possam
ler ou escrever informações, o conceito de
computador digital com programa armazenado não pode ser implementado.
 A CPU processa instruções que são obtidas na MP e os resultados são retornados à MP.
<br><br><br>
Memória Principal 
 A unidade básica de memória é o bit (binary digit)
 Abstração de valores 0 ou 1
 Fisicamente é mais fácil distinguir entre dois valores distintos do que de mais valores. Tensão, corrente, ...
 A memória é formada por um conjunto de células (ou
posições), cada uma das quais podendo guardar uma informação.
 Todas as células de uma dada memória têm o mesmo número de
bits
 Os números que identificam (referenciam) a posição da célula na memória são chamados de Endereços.
 A célula é a menor unidade endereçável da memória
 Endereços são indexadores pelos quais os programas podem referenciar dados na memória.
<br><br><br>

 A memória é formada por um conjunto de células
 Todas as células de uma memória têm o mesmo no de bits
 Cada célula tem um endereço

[Link completo de onde foram tiradas as informações das memórias](http://www.inf.furb.br/~maw/arquitetura/aula4.pdf)











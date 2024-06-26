---
title: Atribuindo Qualidades Mentais a Máquinas
author: 
- John McCarthy (autor)
- P. Schreiber (tradutor)
keywords: 
abstract: |
  Atribuir qualidades mentais como _crenças_, _intenções_ e _vontades_ a uma máquina é às vezes
  correto, quando feito de forma conservadora, e necessário para expressar o que se sabe sobre
  seu estado. Propomos para isso novas ferramentas definicionais: definições relativas a uma
  teoria aproximada, e definições estruturais de segunda ordem.
---

# Introdução

Atribuir certas _crenças, conhecimento, livre-arbítrio, intenções, consciência, habilidade 
ou vontades_ a uma máquina ou programa de computador é legítimo quando tal atribuição expressa
a mesma informação sobre a máquina que expressa sobre uma pessoa. É útil quando a atribuição
ajuda-nos a entender a estrutura da máquina, seu comportamento passado ou futuro, como reparar
ou melhorá-la. Não é talvez jamais logicamente necessário mesmo para humanos, mas expressar
razoável e brevementeo que sabe-se sobre o estado de uma máquina em uma situação particular
pode exigir atribuir a elas qualidades mentais ou qualidades isomórficas[^1]. Teorias sobre a
crença, o conhecimento e o vontade podem ser elaboradas a respeito de máquinas de forma mais
simples do que a respeito de humanos, e em seguida aplicadas a humanos. A atribuição de
qualidades mentais é mais direta e imediata para máquinas de estrutura conhecida, como
termostatos e sistemas operacionais de computadores, mas é mais útil quando aplicada a entidades
cuja o conhecimento sobre sua estrutura é incompleto.

[^1]: McCarthy e Hayes (1969) definem como uma representação da informação _epistemologicamente
adequada_ aquela que expressa a informação de fato presente para um sujeito em quaisquer 
circunstâncias. Assim, quando vemos uma pessoa e partes dela estão encobertas, utilizamos 
a memória de visões anteriores e o conhecimento deral sobre os seres humanos para completar
uma "figura" composta de informações de suas e três dimensões. Devemos também considerar
representações _metafisicamente adequadas_, que representam fatos completos que ignoram
a habilidade do sujeito de captar os fatos em certas circunstâncias. Laplace pensava que as 
posições e velocidades das partículas no universo proporcionavam uma representação 
metafisicamente adequada. Tais representações são necessárias para teorias científicas, mas a
inteligência artificial e a investigação filosófica da experiência do senso comum também requer
representações epistemologicamente adequdas. Este artigo pode ser sintetizado como um argumento
de que conceitos mentais são necessários para uma representação epistemologicamente adequada de
dados sobre as máquinas, especialmente as futuras máquinas inteligentes.

Ainda que sejamos liberais ao atribuir _algumas_ qualidades mentais até para máquinas
primitivas, tentaremos ser conservadores quanto aos nossos critérios para atribuir qualquer
qualidade _particular_.

Estas teses são motivadas pelo trabalho em inteligência artificial[^2] (IA). Elas declaram que
muitos problemas filosóficos a propósito da mente tomam forma concreta quando consideramos
seriamente a ideia de fazer máquinas comportarem-se inteligentemente. Em particular, IA levanta,
a respeito de máquinas, dois problemas até agora considerados restritos ao domínio humano.

[^2]: A investigação sobre a inteligência artificial ainda está longe de apresentar como
alcançar uma performance de nível humano. Nossa abordagem para o problema da IA envolve
identificar os mecanismos necessários para solucionar problemas e descrevê-los precisamente.
Portanto, estamos na ponta do espectro filosófico que requer que tudo seja formalizado em
uma lógica matemática. Diz-se às vezes que o estudo da filosofia serve para superar uma
visão de mundo ingênua ou ignorante; mas para a inteligência artificial, infelizmente, ninguém
conseguiu ainda descrever mesmo uma visão de mundo rudimentar, de forma completa e precisa o
suficiente para permitir construir um programa de aprendizado.

Primeiramente, ao desenhar programas inteligentes e avaliá-los de uma perspectiva exterior,
precisamos determinar as condições sob as quais são aplicáveis termos mentais e volitivos.
Podemos exemplificar esse problema perguntando quando é legítimo dizer, a respeito de uma
máquina: _"ela sabe que eu quero uma passagem para Boston, e pode me dar, mas não me dará."_

Em segundo lugar, quando queremos um programa de computador _genericamente inteligente_[^3],
devemos definir nele uma intuição genérica sobre o mundo, com atenção especial para fatos sobre
como a informação necessária para resolver preblemas deve ser obtida e utilizada. Devemos
portanto determinar uma _metafísica_ (intuição genérica) e uma _epistemologia_ 
(teoria do conhecimento), ainda que rudimentar.

[^3]: Programas de inteligência artificial atuais operam em domínios limitados, e.g. jogos,
provas de teoremas em sistemas lógicos particulares, sentenças de linguagem natural sobre
assuntos específicos e com restrições semânticas. A inteligência artificial genérica requer
modelos genéricos de situações que se transformam com o tempo, agentes com objetivos e
estratégias para atingi-los, e conhecimento sobre como a informação pode ser adquirida.

Tanto quanto possível, atribuímos qualidades mentais distintas umas das outras, em vez de
empacotá-las em um conceito de _mente_. Isso é necessário porque as máquinas atuais
têm mentes pequenas e variadas. As qualidades mentais que podemos atribuir a elas são poucas,
e variam de máquina para máquina. Não tentaremos nem mesmo responder a objeções como _"se não for
capaz também de X, é ilegítimo falar de suas capacidades mentais."_

Podemos dizer que máquinas simples como termostatos têm crenças, e ter crenças parece ser uma
característica comum da maioria das máquinas capazes de resolver problemas. Entretanto, as
máquinas consideradas úteis de serem construídas pelos humanos até o momento raramente têm  
crenças sobre crenças, mesmo que tais crenças sejam necessárias para tornar programas capazes de
cogitar sobre o conhecimento que lhes falta e como adiquiri-lo. Qualidades mentais particulares
a estruturas motivacionais humanas[^4], como amor e ódio, não são necessárias para o
comportamento inteligente, mas nós conseguiríamos provavelmente programar computadores para
exibi-las, se quiséssemos, uma vez que nossas noções de senso comum sobre elas traduzem-se
diretamente em certos programas e estruturas de dados. Outras qualidades mentais, e.g. humor,
apreciação estética, são muito mais difíceis de modelar.

[^4]: Nossa opinião é que a estrutura da inteligência humana é determinada substancialmente
pelos problemas intelectuais enfrentados pelos humanos. Da mesma forma, um marciano ou uma
máquina necessitaria de tais estruturas para resolver tais problemas. Dennett (1971) expressa
opiniões semelhantes. Por outro lado, as estruturas motivacionais humanas parecem ter diversos
aspectos não encontrados em marcianos, e que não teríamos razão para programar em máquinas.
Não precisamos neste artigo apresentar argumentos a favor desta opinião.

As próximas seções deste artigo oferecerão: razões, segundo o estudo da filosofia e da IA,
para atribuir crenças a máquinas; duas novas formas de definição necessárias para definir
qualidades mentais, e exemplos de seu uso; exemplos de sistemas aos quais atribuímos qualidades
mentais; primeiras tentativas de definir várias qualidades mentais; comentários sobre outras 
opiniões a respeito das qualidades mentaisr; notas e referências.

Este artigo é exploratório, e sua apresentação é não-técnica. Quaisquer axiomas apresentados são
ilustrativos, e não fazem parte de uma proposta de um sistema axiomático rigoroso para IA ou
para a filosofia. Isto é indesejável por duas razões: primeiro, a apreensão desses
conceitos para IA requer o estabelecimento formal de axiomas; segundo, a ausência de
formalismos faz com que se dê mais atenção a saber se definimos corretamente as diferentes
qualidades mentais, e não às propriedades formais das teorias apresentadas. Comparemos com
a seguinte situação dos fundamentos da matemática, em que as controvérsias sobre os pontos
de vista clássico ou intuicionista foram suplantadas por estudos técnicos de teorias clássicas
ou intuicionistas, e as relações entre eles. Em trabalhos futuros, espero tratar desses
assuntos formalmente, como em [TODO] (McCarthy 1977) e (1979). Não será possível eliminar as
controvérsias a respeito da verdadeira natureza das qualidades mentais, e acredito que a
resolução definitiva requer mais conhecimento técnico do que existe hoje.

# Por que atribuir qualidades mentais

Por que deveríamos atribuir qualidadades mentais a máquinas? Esta é a questão
oposta à do reducionismo. Em vez de perguntarmos como as qualidades mentais
podem ser reduzidas a qualidades físicas, perguntamos como atribuir qualidades
mentais a sistemas físicos.

Nossa motivação geral para atribuir qualidades mentais é a mesma que a para
atribuir quaisquer outras qualidades: expressar informações disponíveis sobre
a máquina e seu atual estado. Para ter informações, devemos ter um espaço de
possibilidades, descritas explicitamente ou não. A atribuição deve portanto
servir para distinguir o estado presente da máquina de estados passados ou
futuros, do estado qem que estaria em outras condições, e do estado de outras
máquinas. Portanto, o problema é se a atribuição de qualidades mentais é útil
para essas distinções no caso das máquinas.

Para definir o problema com mais precisão, consideremos um programa de
computador para o qual possuímos todo o código-fonte[^5]. O comportamento do
programa em qualquer ambiente é determinado pela estrutura do programa e pode
ser desvendado simulando a ação do programa e do ambiente, sem precisar
lançar mão de qualquer conceito de crença. Mesmo assim, há várias razões para
atribuir a crença e outras qualidades mentais:

[^5]: _complete listings_, programas de computador impressos em linguagem
de programação.

1. Mesmo que conheçamos o programa, seu estado em determinado momento não é
diretamente observável, e os fatos que podemos apreender sobre seu estado
atual podem ser, mais do que de qualquer outro modo, prontamente expressos 
atribuindo certas crenças e objetivos.
2. Mesmo que possamos simular sua interação com o ambiente por meio de outro
programa mais compreensível, a simulação pode ser um bilhão de vezes mais lenta.
Podemos também não ter acesso às condições iniciais do ambiente ou às leis 
de movimento de forma adequada, ao passo que podemos prever os efeitos das
crenças que atribuímos ao programa sem a presença de um computador físico.
3. Atribuir crenças permite derivar enunciados gerais sobre o comportamento
do programa que não poderiam ser obtidos de qualquer número finito de simulações.
4. As estruturas de crenças e objetivos que atribuímos a programas podem ser 
mais fáceis de compreender que os detalhes do programa expressos no código-fonte.
5. A estrutura de crenças e objetivos é presumivelmente mais próxima da estrutura
mental concebida pelo programador[^6]; portanto, pode ser mais fácil 
corrigir[^7] o programa em termos desta estrutura do que diretamente pelo 
código-fonte. De fato, é frequente que corrijam-se falhas raciocinando em 
termos gerais sobre as informações de um programa ou máquina, diagnosticando 
quais são as crenças falsas, e procurando nos detalhes de um programa ou 
máquina apenas o suficiente para determinar como crenças falsas são 
representadas e quais mecanismos causam seu surgimento.
6. A diferença entre um programa e outro programa real ou hipotético pode ser
melhor expressada como uma diferença de estruturas de crenças.

[^6]: _designer of the program_.
[^7]: _debug_.

Todas as razões acima para atribuir crenças são epistemológicas; i.e., 
atribuir crenças é necessário para adaptar as limitações da nossa habilidade 
de adquirir conhecimentos, fazer previsões, e estabelecer generalizações em
termos das estruturas fundamentais de programas. Talvez esta seja a razão geral
para atribuir altos níveis de organização a sistemas[^8].

[^8]: linguagens de alto nível, abstrações.

Computadores dão ensejo ao surgimento de vários exemplos de como construir
estruturas de alto nível com base em estruturas de baixo nível, e de como
fazer análises utilizando as estruturas de alto nível. A geometria de campos
elétricos em um transistor e sua composição química determinam suas propriedades
como elementos de um circuito elétrico. Transistores são combinados em pequenos
circuitos e alimentados segundo padrões que constituem elementos lógicos como
_ANDs_, _ORs_, _NOTs_, e _flip-flops_. Computadores são desenhados com esses
componentes lógicos de forma a obedecer certas operações do processador[^9]; 
o arquiteto do sistema normalmente não precisa considerar as propriedades dos 
transistores como elementos do circuito. Ao escrever um compilador a partir de 
uma linguagem de alto nível, trabalhamos com as operações do processador sem
precisar conhecer os _ANDs_ e _ORs_; o usuário de uma linguagem de alto nível
não precisa conhecer as operações do processador de um computador.[^10]

[^9]: _order code_, e.g. operações definidas em assembly language.
[^10]: McCarthy descreve aqui o procedimento que convencionou-se chamar de 
_abstração.

Nos casos descritos acima, usuários do alto nível podem ignorar completamente
o baixo nível, porque o comportamento do alto nível é totalmente determinado
pelos valores de variáveis de alto nível; e.g., para determinar o resultado de
um programa de computador, não é necessário levar em consideração os 
_flip-flops_ da máquina. Entretanto, quando atribuímos estruturas mentais a 
humanos ou objetivos para a sociedade, sempre produzimos sistemas incompletos;
o comportamento de alto nível não pode ser totalmente previsto por observações
e leis de alto nível, mesmo quando o comportamento de baixo nível é determinado.
Além disso, em um dado estado da ciência e da tecnologia, diferentes tipos de
informação podem ser obtidos a partir da experiência e da construção de teorias
em diferentes níveis da organização.

Para programar um computador que obtenha informações e coopere com pessoas e
outras máquinas, precisamos fazer com que atribua conhecimento, crenças e
vontades em outras máquinas e pessoas. Por exemplo, um programa que planeje
viagens deverá atribuir cohecimento a agentes de viagem e computadores de
reserva de companhias aéreas. Deverá de alguma maneira tratar as informações
nos registros, talvez atribuindo a eles uma forma passiva de conhecimento.
Quanto mais poderoso for o programa para interpretar o que lhe é dito, menos
precisará conhecer sobre como a informação que recebe é representada
internamente em sua fonte, e mais suas atribuições de conhecimento parecer-se-ão
com as atribuições de conhecimento de um ser humano a outro.

# Dois métodos de definição e sua aplicação a qualidades mentais

Em nossa opinião, uma grande fonte de problemas para definir conceitos mentais
e intensionais[^11] é a fraqueza dos métodos de definição _explicitamente_
utilizados. Introduzimos aqui dois tipos de definição: _definição relativa a uma teoria aproximada_
e _definição estrutural de segunda ordem_, aplicando-as à definição de qualidades mentais.

[^11]: _intensional_, termo lógico-filosófico que significa a descrição de um
objeto por suas propriedades, e não por sua identidade (sua existência mesma).

## Definições relativas a uma teoria aproximada

É consenso que a maioria dos conceitos científicos não são definidos por 
sentenças em linguagem natural, mas como partes de teorias, e que a aceitação
da teoria é definida por sua conformidade a uma coleção de fenômenos. Propomos
um método similar para explicar conceitos mentais e outros conceitos do senso
comum, mas um fenômeno particular tem um papel mais importante do que no caso de
teorias científicas: o conceito só é relevante no interior de uma teoria, 
e não pode ser definido com mais precisão do que essa teoria permite.

A noção de uma teoria aproximada de outra precisa ser formalizada. No caso
da física, podemos pensar em vários tipos de aproximação numérica ou probabilística.
Penso que este tipo de aproximação seja atípica e errônea, e não ajude a explicar
conceitos como _ação intencional_ de forma significativa e relevante a teorias
aproximadas. Em vez disso, pode desenrolar-se como: 

Consideremos uma teoria detalhada $T$ com uma variável de estado $s$. Podemos
imaginar que $s$ muda com o tempo. A teoria aproximada $T'$ tem uma variável
$s'$. Há um predicado $atp(s, T')$ cuja verdade significa que $T'$ se aplica
quando o mundo está em um estado $s$. Há uma relação $corr(s, s')$ que afirma
que $s'$ corresponde ao estado $s$. Temos:

$$ \forall s.(atp(s, T') \rightarrow \exists s'.corr(s, s')).$$

Certas funções $f_1(s)$, $f_2(s)$, etc. têm funções correspondentes $f'_1(s')$,
$f'_2(s')$, etc. Temos relações como:

$$ \forall ss'.(corr(s, s') \rightarrow f1(s) = f1' (s')).$$

Entretato, a teoria aproximada $T'$ pode ter funções adicionais $g'_1(s')$, etc.
que não correspondem a nenhuma função de $s$. Mesmpo quando for possível construir
$gs$ correspondentes a $g's$, as definições frequentemente parecerão arbitrárias,
porque o uso de $g'_1$ pelo senso comum restringir-se-á ao contexto $T'$. 
Exemplos disso são conceitos cujas definições envolvem contrafatuais.

Suponhamos que se queira atribuir _intenção_ e _livre-arbítrio_, e distinguir
uma _ação deliberada_ de uma ocorrência. Chamaremos um resultado de _ação deliberada_ 
se o resultado fosse ser diferente se as intenções da máquina fossem diferentes.
Isso requer um critério para a verdade da sentença condicional contrafatual
_"se as intenções fossem diferentes, o resultado não teria ocorrido"_, tornando
assim necessária uma nova abordagem para uma classe importante de contrafatuais.

Tratamos o _aspecto relevante da realidade_ como um produto cartesiano para que
possamos falar sobre a mudar um componente deixando os outros inalterados.
Isso seria razoável se a estrutura de produtos cartesianos existisse no mundo;
entretanto, ela existe apenas em certos modelos aproximados do mundo. Portanto,
nenhum estado do mundo como um todo, definido e único, corresponde à mudança
de um componente. O parágrafo seguinte apresenta essas ideias em mais detalhes.

Suponhamos que $A$ seja uma teoria na qual algum aspecto da realidade é
caracterizado pelos valores de três quantidades $x$, $y$ e $z$. Consideremos
$f$ como uma função de três argumentos, e $u$ uma quantidade tal que 
$u = f(x,y,z)$, onde $f(1,1,1) = 3$ e $f(2,1,1) = 5)$. Consideremos então um
estado do modelo em que $x = 1$, $y = 1$, e $z = 1$. No interior da teoria $A$,
a sentença condicional contrafatual _"u = 3, mas se x fosse 2, então u seria 5"_ 
é verdadeira, porque a condição contrafatual contempla mudar x para 2 e deixar
as outras variáveis inalteradas.

Agora superemos esse modelo supondo que $x$, $y$ e $z$ são quantidades que
dependem do estado do mundo. Mesmo se $u = f(x,y,z)$ for tomado como uma
lei da natureza, o contrafatual não precisa ser tomado como verdade,
porque alguém pode argumentar que se $x$ fosse 2, então $y$ seria 3, para que
$u$ não seja 5. Se a teoria $A$ tiver um estado _suficientemente preferido_,
podemos tomar o significado do contrafatual de $A$ como seu significado geral,
mas às vezes pode ser melhor considerar o contrafatual definido na teoria,
i.e. como _sincategoremático_, no jargão kantiano.

Um exemplo do senso comum pode ajudar: suponhamos que um instrutor de esqui diga
"ele não teria caído se tivesse dobrado os joelhos ao fazer aquela curva", e
outro instrutor responda "não, ele caiu porque não pôs o peso no esqui na descida".
Suponhamos ainda que, ao assistir a uma filmagem, eles concordem que o primeiro
instrutor estava correto e o segundo incorreto. Eu argumento que essa concordância
se baseia em uma aceitação comum de uma teoria do esqui, e que no interior da teoria,
a decisão pode se rigorosa mesmo se ninguém imagina um mundo alternativo tão
semelhante quanto possível ao mundo real, mas em que o aluno tivesse posto
o peso no esqui na descida.

Propomos que este é frequentemente (e ainda não busquei contraexemplos) o
significado, segundo o senso comum, de contrafatuais. O contrafatual tem um
significado definido em uma teoria, porque a teoria tem uma estrutura de 
produto cartesiano, e a teoria é suficientemente preferida, de tal forma que
o significado do contrafatual no mundo é tomado como seu significado na teoria.
Isso é especialmente verdadeiro no caso de conceitos que têm uma definição natural
em termos de contrafatuais, e.g. o conceito de _ação deliberada_, com que iniciamos
esta seção.

Em todos os casos que conhecemos, a teoria é aproximada e incompleta. Tomadas certas
premissas como verdadeiras, uma certa quantidade é aproximadamente uma função de 
outras quantidades. A incompletude se deve à teoria não prever os estados do mundo,
mas apenas algumas funções deles. Assim, um conceito útil como a ação deliberada
parece desaparecer quando examinaddo de perto, e.g. quando tentamos defini-lo
em termos de estados do mundo, e não em termos de certas funções desses estados.

### Observações

1. Os casos conhecidos em que um conceito é definido
   em relação a uma teoria aproximada envolvem contrafatuais.
   Isso pode não ser sempre o caso.
2. É importante estudar a natureza das aproximações.
3. McCarthy e Hayes (1969) tratam a noção de _X pode fazer Y_
   usando uma teoria em que o mundo é entendido como uma grupo
   de autômatos interagindo entre si. O artigo não leva em consideração
   que sentenças com "podem" não podem ser traduzidas em afirmações
   simples sobre o mundo.
4. A tentativa de uma psicologia introspectiva obsoleta
   de analizar a mente em termos da interação da _vontade_,
   _intelecto_ e outros componentes não pode ser excluida pelas razões
   metodológicas usadas pelos _behavioristas_ e positivistas para
   classificá-las como sem sentido e excluí-las da ciência. Esses
   conceitos podem ter definições precisas em uma teoria aproximada adequada.
5. A abordagem sobre contrafatuais em que são definidos em termos de
   estruturas de produtos cartesianos de uma teoria aproximada
   podem ser melhores do que a abordagem do _mundo possível mais próximo_, 
   de Lewis (1973). Os valores-verdade são bem definidos no interior
   de teorias aproximadas, e as teorias podem ser justificadas
   por evidências envolvendo fenômenos não mencionados em afirmações
   contrafatuais isoladas.
6. Definições relativas a teorias aproximadas podem ajudar
   a separar questões, como as que envolvem contrafatuais,
   em questões _internas_ à teoria aproximada e questões _externas_ 
   à justificativa da teoria como um todo. Podemos presumir que as
   questões internas sejams técnicas e tenham respostas definidas para que
   as pessoas concordem, mesmo que tenham discordâncias científicas 
   ou filosóficas sobre as questões externas.

## Definições estruturais de segunda ordem

Definições estruturais de qualidades são dadas em termos do estado do sistema
descrito, ao passo que definições comportamentais são dados em termos de seu
comportamento atual ou potencial[^12].

[^12]: _Nota do tradutor:_ Definições comportamentais são comuns na 
filosofia. Dizemos que um sistema tem uma certa qualidade se ele se comporta de
uma certa maneira ou está _disposto_ a se comportar de certa maneira. É uma
postura conservadora, que não afirma estados internos inobserváveis pela
ciência atual, e que podem manter-se inobserváveis. Entretanto, tais definições
são inadequadas para qualidades mentais, porque, como o senso comum sugere,
uma qualidade mental pode não resultar em um comportamento, dado que outra
qualidade mental pode impedi-lo; e.g., posso pensar que alguém é teimoso, mas
a cortesia me impede de dizê-lo. Certas dificuldades podem ser superadas, mas 
a ideia permanece vaga. A preferência por definições comportamentais se dá
por precaução, mas na minha interpretação as experiências científicas mostram
que a audácia ao postular estruturas complexas de entidades inobserváveis --
desde que acompanhada da disposição para desfazer erros -- tem mais chances de
ser recompensada com o entendimento e o controle da natureza do que a timidez
positivista. É particularmente instrutivo imaginar um _behaviorista_ determinado
tentando compreender um computador eletrônico. Tentar definir cada qualidade
por meio de uma abordagem comportamental não o levaria a lugar algum; apenas
postulando simultaneamente uma estrutura complexa que incluísse memória,
unidade aritmética, estruturas de controle, e entrada e saída (IO) produziria
conjecturas comparáveis às experiências. 

    Há um sentido em que as definições operacionais não são tomadas seriamente
mesmo por seus adeptos. Suponhamos que alguém dê uma definição operacional do
comprimento (e.g. utilizando uma barra de platina), e toda uma escola de físicos
e filósofos tornem-se a ela apegados. Alguns anos depois, alguém critica a
definição, afirmando carecer de alguma qualidade desejável, e propões uma
alteração que é aceita. Essa situação é normal, mas se a definição original
expressasse mesmo o significado de comprimentro, a mudança não teria sido 
aceita, e ter-se-ia argumentado que, embora possivelmente útil, não expressaria
o que se quer dizer por "comprimento. Isso mostra que o conceito de comprimento
como uma propriedade dos objetos é mais estável do que qualquer definição
operacional.

    Carnap tem uma seção interessante em Significado e Necessidade (Meaning
and Necessity) intitulado "O conceito de intensão para um robô", em que
argumenta um ponto semelhante, dizendo: "É claro que o método de análise
estrutural, se aplicável, é mais poderoso do que o método comportamental,
porque pode proporcionar uma resposta geral, e, em circunstâncias favoráveis,
até uma resposta completa para a questão da intensão de um dado predicado."

    O argumento decisivo para a inteligência artificial (AI), entretanto, é
um argumento arquitetônico ("argument from design"). A fim de produzir um
comportamento desejado em um computador, desenhamos certas qualidades mentais
em sua estrutua. Isso não leva a caracterizações comportamentais de suas
qualidades, porque as qualidades particulares são apenas uma das diversas
formas por meio das quais podemos obter o comportamento desejado, e de toda
forma o comportamento pode nem sempre se realizar.

Se a estrutura da máquina for conhecida, pode-se oferecer uma _definição estrutural de primeira ordem ad hoc_.
Trata-se de um predicado $B(s,p)$ em que $s$ representa o estado da máquina,
$p$ representa uma sentença em uma linguagem adequada, e $B(s,p)$ é a afirmação
de que quando a máquina estiver em um estado $s$, ela _crê_ na sentença $p$.
As considerações deste artigo são neutras quanto a considerar o objeto da crença
como uma sentença, usar um operador modal, ou admitir _proposições_ como objetos
críveis. Escrevemos este artigo tomando sentenças como objetos da crença, mas
recentemente passei a preferir as proposições, e discuto-as em outro texto (McCarthy, 1979).

Uma definição estrutural de _primeira ordem_ de crença seria um predicado
$B(W,M,s,p)$ em que $W$ fosse o mundo em que a máquina $M$ em questão estaria
situada. Não posso dizer como oferecer uma tal definição de crença, e penso
ser impossível. Portanto, devemos conformar-nos com definições de segunda ordem[^13].

[^13]: Putnam (1970) também propõe definições de segunda ordem para
propriedades psicológicas.

Uma definição estrutural de segunda ordem de crença é um predicado de segunda
ordem $\beta(W,M,B)$, que afirma que o predicado de primeira ordem $B$ é uma
boa noção que a máquina $M$ tem no mundo $W$. _Boa_ significa que as crenças
que $B$ atribui a $M$ estão de acordo com as nossas ideias sobre quais crenças
$M$ teria, e não que as crenças são em si mesmas verdadeiras. A axiomatização
de crenças disponíveis na literatura são definições de segunda ordem parciais.

Em geral, definições de segunda ordem oferecem critérios para avaliar a atribuição
de qualidades a um sistema. Propomos que nosso senso comum e o uso científico
de qualidades não diretamente observáveis correspondem com menos rigor a
definições estruturais de segunda ordem do que a qualquer tipo de definição comportamental. 
Notemos que uma definição de segunda ordem não garante que existam predicados $B$ que
satisfaçam os critérios $\beta$, ou que $B$ seja único. Algumas qualidades são
melhor definidas em conjunto com outras qualidades relacionadas, e.g. 
crenças e objetivos podem precisar de uma abordagem conjunta.

Definições de segunda ordem criticam estruturas de crença inteiras, em vez de
crenças individuais. Podemos trabalhar com crenças idividuais dizendo que um sistema
crê em $p$ em um estado $s$, dado que todo bom $B$ satisfaça $B(s,p)$. Assim,
distinguimos a interseção de todos os bons $B$.

Uma analogia com a criptografia pode ser útil. Resolvemos um criptograma
propondo hipóteses sobre a estrutura da cifra e sobre  a tradução de partes 
do texto da cifra. Nossa solução estará completa quando adivinharmos o sistema
da cifra que produz o criptograma de uma mensagem em texto cru. Mesmo que nunca
provemos que nossa solução é a única, duas soluçoes diferentes quase nunca são
encontradas, exceto para criptogramas curtos. Em uma analogia, a definição de
segunda ordem $\beta$ corresponde à ideia geral de cifragem, e $B$ é o sistema
específico utilizado. Mesmo que raramente possamos provar a unicidade, não
esperamos encontrar dois $B$ que satisfaçam $\beta$. O artigo MH69 discute
a improbabilidade de existirem duas boas decomposições de um autômato em
subautômatos.

Parece-me que deveria haver um metateorema da lógica matemática que afirme que
nem todas as definições de segunda ordem podem ser reduzidas a definições de
primeira ordem, e ainda teoremas que caracterizem as definições de segunda ordem
que aceitam tais reduções. Esses resultados técnicos, se puderem ser produzidos,
podem ser proveitosos à filosofia e à construção de teorias científicas formais.
Especulo que diversos argumentos filosóficos informais de que certos conceitos
mentais não podem ser reduzidos à física reduzir-se-ão a esboços de argumentos
de que tais conceitos necessitam de definições de segunda ordem.

Eis uma definição de segunda ordem aproximada de crença. Para cada estado $s$
da máquina e cada sentença $p$ em uma linguagem adequada $L$, atribuimos verdade
a $B(s,p)$ se e apenas se considerarmos que a máquina crê em $p$ quando está
no estado $s$. A linguagem $L$ é escolhida para a nossa conveniência, e não
assumimos que a máquina represente explicitamente sentenças em $L$. Assim,
podemos falar em crenças de chineses, cães, empresas, termostatos e sistemas
operacionais de computadores, sem assumir que utilizam o inglês ou qualquer
linguagem de primeira ordem que prefiramos. $L$ pode ou não ser a linguagem que
utilizamos para fazer afirmativas; e.g. podemos, escrevendo em inglês, utilizar
sistematicamente sentenças em francês como objetos de crença. Entretanto,
a melhor opção para trabalhar com a inteligência artificial deve ser fazer de
L um subconjunto de uma linguagem _externa_, restrita de tal forma a evitar
autorreferências paradoxais (Montague, 1963).

Devemos aplicar a $B(s,p)$ certos critérios, i.e., $\beta(B,W)$ é verdadeiro
dado que as seguintes condições são satisfeitas:

1. O conjunto $Bel(s)$ de crenças, i.e. o conjunto de $p$ para que $B(s,p) é
dito verdadeiro quando $M$ está em um estado $s$ contém consequências 
suficientemente óbvias de alguns de seus membros.
2. $Bel(s)$ muda de forma razoável quando o estado se modifica com o tempo.
Queremos que novas crenças sejam consequências lógicas ou plausíveis de crenças
anteriores, ou que sejam resultado de _comunicação_ em alguma linguagem de
entrada ^[_input lines_], ou que sejam _observações, i.e. crenças sobre o ambiente
sobre as quais as informações são recebidas como entrada.
3. Preferimos que o conjunto de crenças seja tão consistente como possível.
Admitimos que a consistência não seja um conceito quantitativo em lógica
matemática -- um sistema é consistente ou não, mas parece que às vezes atribuímos
conjuntos de crenças inconsistentes a máquinas ou a pessoas. Nossa intuição diz
que devemos ser capazes de manter certas zonas de consistência em nossas crenças,
e deve ser especialmente importante evitar inconsistências nas crenças puramente
analíticas da máquina.
4. Nossos critérios para sistemas de crenças podem ser fortalecidos se identificarmos
algumas das crenças da máquina como expressões de objetivos; crenças como
"seria bom se". Então, poderíamos dizer que o comportamento da máquina é de
alguma forma _racional_, i.e., _ela faz aquilo que acredita que a a levará a cumprir seus objetivos_.
Quanto mais conseguirmos explicar seu comportamento nesses termos, melhor nos parecerá
a função $B(s,p). Também gostaríamos de interpretar as mudanças de estado intero
como mudanças de crenças, tão quanto isso for razoável.
5. Se a máquina se comunica, i.e. emite em alguma linguagem sentenças que podem
ser interpretadas como afirmações, questões e comandos, gostaríamos que essas
afirmativas estivessem entre suas crenças, a não ser que atribuamo-lha um objetivo
como mentir. Satisfaremo-nos com nossa atribuição de crenças se pudermos
interpretar sua capacidade de comunicação como parte dos objetivos atribuídos.
6. Será proveitoso atribuir crenças introspectivas, e.g. a crença de que não
sabe como voar até Boston, ou mesmo que não sabe o que quer em uma certa
situação.
7. Finalmente, preferiremos uma atribuição $B$ mais econômica a uma menos econômica.
Quanto menos crenças atribuirmos, e quanto menos elas mudarem como consequência de
mudanças de estados e comportamentos, melhor. Em particular, se
$\forall sp.(B1(s,p) \rightarrow B2(s,p))$, mas não o contrário, e B1 contemplar
todas as mudanças de estado e resultados ^[_outputs_] de B2, preferiremos $B1$ a $B2$.
Isso garante que preferiremos não atribuir crenças a pedras, que não mudam de estado
e não têm comportamentos. Um predicado-crença que se aplica a uma coleção de máquinas
é preferível a um que se aplique a apenas uma máquina.

Os critérios acima foram formulados de forma vaga. Isso seria ruim se houvesse
um enorme rol de difentes atribuições de crenças a uma máquina em particular
adequadas aos nossos critérios, ou se esses critérios permitissem atribuições
muito diferentes das nossas intuições. Minha opinião é que um maior esforço
intelectual tornará esses critérios mais precisos, sem um custo de aplicabilidade;
mas ele permanecerão vagos, i.e., ainda atribuiremos crenças a grupos de casos.
Entretanto, da forma vaga como tratamos o assunto hoje, não deve haver atribuições 
de crenças para sistemas de interesse prático devidamente _boas_ que sejam
radicalmente diferentes. Se houvesse, teríamos notado ambiguidades irresolúveis
em nossas atribuições de crenças. Embora não queiramos fixar nossa ideia geral
de crença a uma única axiomatização, precisamos desenhar axiomatizações precisas
de crenças e outras qualidades mentais aplicadas a programas de computador inteligentes.

# Exemplos de sistemas com qualidades mentais

Consideremos alguns exemplos de máquinas e programas aos quais podemos atribuir
estruturas como crenças e objetivos.

## Termostatos

Atribuir crenças a simples termostatos é desnecessário para o estudo dos
termostatos, porque sua operação pode ser muito bem entendida sem isso.
Entretanto, sua própria simplicidade torna claro o que está envolvido nessa
atribuição, e defendemos (em parte como uma provocação àqueles que encaram a
atribuição de crenças a máquinas como uma mera brincadeira) que ela é legítima[^14]

[^14]: Dizer que um sistema tem crenças ou outras qualidades mentais não é
primeiramente uma questão de complexidade do sistema. Embora carros sejam mais
complexos do que termostatos, é difícil atribuir-lhes crenças ou objetivos;
o mesmo talvez seja verdade no caso das peças básicas [_basic hardware_] de um
computador, i.e., a parte do computador que executa o programa, sem o programa
em si.

Primeiro, consideremos um simples termostato que desliga o aquecimento quando
a temperatura atinge um nível acima do configurado, liga o aquecimento quando
a temperatura atinge um nível abaixo do desejado, e deixa aquecimento como está
quando a temperatura está em uma faixa de variação de dois graus acima ou abaixo
do desejado. O predicado mais simples $B(s,p)$ atribui crenças a apenas três
afirmações: "o quarto está muito frio", "o quarto está muito quente", e
"o quarto está confortável" -- crenças atribuídas ao termostato de forma óbvia.
Ainda, atribuimos a ele o objetivo: "o quarto deve permanecer confortável".
Quando o termostato crê que o quarto está frio ou quente demais, ele envia uma
mensagem dizendo isso ao aquecedor. Um predicado de crença mais complexo poderia
também ser definido, no qual o termostato tem uma crença sobre qual deveria ser
a temperatura, e outra crença sobre qual ela é. Não é claro qual é melhor, mas
se desejarmos levar em conta possíveis erros no termômetro, então precisaremos
atribuir crenças sobre qual é a temperatura. Não atribuímos quaisquer outras crenças:
o termostato não tem opiniões sobre o termostato estar ligado ou desligado,
sobre o tempo lá fora, ou sobre quem venceu a batalha de Waterloo. Além disso,
não tem crenças introspectivas, i.e., não crê crer que o quarto está quente demais.[^15]

[^15]: Crenças a respeito de o quarto estar quente demais, etc. são atibuídas
a um termostato ligado e configurado; o termostato dentro da caixa não tem
crenças ainda, e pode ser usado de outas maneiras e com crenças diferentes.

Comparemos $B(s,p)$ acima com os critérios da seção anterior. A estrutura de crença
é consistente (porque todas as crenças são independentes umas das outras), elas
surgem da observação, e resultam em ações de acordo com os objetivos atribuídos.
Não há um raciocínio, mas apenas comandos (que não incluímos em nossa discussão)
que são comunicados. Claramente, neste caso, atribuir crenças é um benefício intelectual
modesto. Entretanto, se considerarmos toda a classe dos termostatos possíveis, 
então a estrutura de crenças atribuída tem uma maior constância comparada 
aos mecanismos para medir e representar a temperatura.

O sistema de controle da temperatura da minha casa pode ser descrito da seguinte
maneira: termostatos nos andares de cima e de baixo dizem ao sistema central
que deve ligar ou desligar o fluxo de água quente para essas áreas. Um termostato
central para a temperatura da água diz ao aquecedor que deve ligar ou desligar,
mantendo assim o reservatório central de água na temperatura correta. Recentemente
estava quente demais no andar de cima, e questionamo-nos se o termostato _cria_
erroneamente que estava frio demais no andar de cima, ou se o termostato do aquecedor
_cria_ erroneamente que a água estava fraia demais. A realidade não era nenhum desses erros:
o controlador do andar de baixo _tentou_ desligar o fluxo de água, mas não _podia_,
porque a válvula estava emperrada. O encanador veio até a casa e descobriu o problema,
e veio novamente quando encomendamos uma peça substituta. Uma vez que os serviços de
encanador estão cada vez mais caros, e microcomputadores estão cada vez mais baratos,
faz sentido desenvolver sistemas de controle de temperatura que _conheçam_ muito mais
sobre o estado térmico da casa, e sobre seu próprio estado de funcionamento.

Em primeiro lugar, embora o presente sistema _não possa_ desligar o fluxo de água
no andar de cima, não há razão para atribuir-lhe o _conhecimento_ de que não possa,
e _a fortiori_ não tem a habilidade de _comunicar_ este _fato_ ou levá-lo em conta
ao controlar o sistema. Um sistema mais avançado saberia se as _ações_ que _tentou_
executar lograram, comunicaria as falhas e adaptar-se-lhes-ia. Adaptamo-nos à falha
desligando o sistema inteiro até que a casa se resfriasse, e então deixando que as
duas partes esquentassem juntas. O sistema atual tem a _capacidade física_
de fazer isso mesmo que não tenha _conhecimento_ ou _vontade_.

Embora o termostato creia que o quarto está frio demais, não há necessidade de
dizer que ele entenda o conceito de frio demais. A estrutura interna de "o quarto
está frio demais" é parte da nossa linguagem, não da sua.

Consideremos um termostato cujos fios que ligam-no ao aquecedor foram cortados.
Podemos ainda dizer que sabe se o quarto está frio demais? Dado que consertar o
termostato pode ser facilitado se atribuirmos esse conhecimento, gostaríamos de
fazê-lo. Nossa justificativa é que somos capazes de distinguir, em nossa linguagem,
o conceito de um sistema de controle de temperatura quebrado do conceito de uma
certa coleção de peças, i.e., fazer caracterizações intensionais de objetos físicos[^16][^17].

[^16]: Tom Costello assinalou que podemos às vezes atribuir conhecimento introspectivo
a sistemas simples. Por exemplo, podemos dizer que um relógio despertador eletrônico
que é ligado depois de estar desligado sabe que não sabe a hora. Ele pede para ser
reconfigurado piscando a tela. O relógio despertador convencional pode ser entendido
da mesma forma por uma perspectiva do design ou uma perspectiva de intenção.
Entretanto, podemos imaginar um alarme despertador que tivesse uma estratégia interessante
para conhecer o tempo após uma falha de energia. Nesse caso, a atribuição de conhecimento
do não conhecimento poderia ser a a melhor maneira para entender essa parte do estado.

[^17]: O sistema de informações de vôo da American Airlines me disse: "sobre qual
cidade você deseja informações de desembarque?". Eu respondi: "São Francisco".
Ao que respondeu: "eu acredito que você disse 'São Francisco'; se isso está correto,
diga 'sim'". Convido as pessoas com resistência em relação a máquinas que dizem "eu" ou "penso"
a proporem sugestões sobre o que o sistema deveria ter dito.

## Configurações inteligentes autorreprodutoras em um mundo celular autômato [TODO: melhorar título]

Um _sistema autômato celular_ atribui um autômato finito a cada ponto do plano
com coordenadas de inteiros. O estado de cada autômato em um tempo $t + 1$
depende de seu estado no tempo $t$ e dos estados dos autômatos vizinhos no
tempo $t$. Um dos primeiros a utilizar o conceito de autômatos celulares foi
Von Neumann, que descobriu um autômato de 27 estados cujas células podiam ser
inicializadas com uma configuração autorreprodutora que funcionava como um
computador universal. O autômato básico no sistema de Von Neumann tinha um
estado de descanso[^ _resting state_] 0, e um ponto em estado 0 cujos quatro
autômatos vizinhos estariam também em estado 0. As configurações iniciais
que consideramos teriam um número finito de células em estado 0 e, é claro,
esta propriedade persiste mesmo que o número de células com valor diferente de
zero cresça indefinidamente com o tempo.

O sistema autorreprodutor usava os estados de uma longa cadeia de células com
valor diferente de zero como uma fita contendo instruções para um construtor
universal que construiria cópias da sequência a ser reproduzida, mas com cada 
célula em um estado passivo que persistiria enquanto os autômatos vizinhos 
estivessem também em estados passivos. Após a fase de construção, a fita seria
copiada para criar a fita da nova máquina, e o novo sistema entraria em 
movimento ativando-se uma das células. O novo sistema então distanciar-se-ia
do sistema-mãe, e o processo começaria novamente. O propósito desse design era
demonstrar que configurações arbitrariamente complexas poderiam ser
autorreprodutoras -- complexidade garantida por serem computadores universais.

Desde o tempo de Von Neumann, foram descobertas formas mais simples de células 
de computadores universais autorreprodutoras. A mais simples até agora,
de autômatos de dois estados, é o Jogo da Vida de John Conway (Gosper, 1976);
para uma descrição completa e detalhada, Poundstone, 1976. O estado de uma
célula no tempo $t + 1$ é determinado por seu estado no tempo $t$ e pelo estado
das oito células vizinhas no tempo $t$. Um ponto cujo estado seja 0 mudará seu
estado para 1 caso exatamente três células vizinhas estejam no estado 1. Um
ponto cujo estado seja 1 permanecerá no estado 1 caso duas ou três células
vizinhas estejam no estado 1. Em todos os outros casos o estado torna-se ou
permanece 0.

Embora não tenha sido esta a razão de Conway para apresentá-los, Conway e Gosper
mostraram que computadores universais autorreprodutores poderiam ser construídos
como configurações do Jogo da Vida. Poundstone (1984) oferece uma descrição
completa do autômato do Jogo da Vida, incluindo computadores universais e
sistemas autorreprodutores.

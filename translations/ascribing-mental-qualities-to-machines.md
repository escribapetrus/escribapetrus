---------------
title: Atribuindo Qualidades Mentais a Máquinas
author: John McCarthy

translated by: P. Schreiber

abstract
Atribuir qualidades mentais como _crenças_, _intenções_ e _apetites_ a uma máquina é às vezes
correto, quando feito de forma conservadora, e necessário para expressar o que se sabe sobre
seu estado. Propomos para isso novas ferramentas definicionais: definições relativas a uma
teoria aproximada, e definições estruturais de segunda ordem.
-----------------

# Introdução

Atribuir certas _crenças, conhecimento, livre-arbítrio, intenções, consciência, habilidade 
ou apetites_ a uma máquina ou programa de computador é legítimo quando tal atribuição expressa
a mesma informação sobre a máquina que expressa sobre uma pessoa. É útil quando a atribuição
ajuda-nos a entender a estrutura da máquina, seu comportamento passado ou futuro, como reparar
ou melhorá-la. Não é talvez jamais logicamente necessário mesmo para humanos, mas expressar
razoável e brevementeo que sabe-se sobre o estado de uma máquina em uma situação particular
pode exigir atribuir a elas qualidades mentais ou qualidades isomórficas[^1]. Teorias sobre a
crença, o conhecimento e o apetite podem ser elaboradas a respeito de máquinas de forma mais
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
oposta à do reducionismo. Em vez de perguntarmso como as qualidades mentais
podem ser reduzidas a qualidades físicas, perguntamos como atribuir qualidades
mentais a sistemas físicos.


































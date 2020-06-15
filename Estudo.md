# Estudo do Projeto

Fonte de 100mA

## Introdução

Neste documento se encontram as informações adquiridas para a montagem da fonte.

## Componentes

### Resistor

O resistor é um dispositivo elétrico que consome corrente elétrica. É utilizado principalmente para limitar a corrente elétrica em um circuito e para converter energia elétrica em energia térmica.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/1-imagem-resistor.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/2-simbolo-resistor.png?raw=true)

Uma equação importante ao trabalhar com resistores é U = R ∙ i (Primeira Lei de Ohm), em que U é a diferença de potencial (em Volts), R é a resistência (em Ohms) e i é a corrente elétrica (em Amperes). A corrente no circuito varia de acordo com a resistência e a tensão.

    Primeira Lei de Ohm: U = R ∙ i

Outra equação importante para entender a grandeza “resistência elétrica”, é a Segunda Lei de Ohm. Na verdade, até um fio apresenta resistência, mas em circuitos simples não é necessário considerá-la.

    Segunda Lei de Ohm: R = (ρ ∙ L)/A

Nesse caso, ρ é uma constante associada ao material, (resistividade do material) L é o comprimento do fio e A é a área da seção transversal do fio.

Resistores combinados em série e em paralelo podem ser substituídos por um resistor equivalente. Caso os resistores sejam ligados em série, a nova resistência será igual à soma das resistências. Em paralelo, o inverso da nova resistência será igual à soma do inverso das resistências.

    Associação em série: Req = R1 + R2 + ⋯

    Associação em paralelo: 1/Req = 1/R1 + 1/R2 + ⋯

É importante notar o que acontece com a tensão e a corrente em circuitos elétricos em série e em paralelo.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/3-circuito-em-paralelo.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/4-circuito-em-serie.png?raw=true)

O circuito em paralelo divide a corrente (nesse caso, i1 + i2 + i3 = i), mas a tensão é a mesma em todos os resistores. Já no circuito em série, a tensão que é dividida (com U1 + U2 + U3 = U), sendo que a corrente que passa por cada um dos resistores é a mesma. O que descreve isso mais formalmente são as Leis de Kirchhoff.

Por esse motivo, para medir tensão, colocamos o voltímetro em paralelo, e para medir corrente, colocamos o amperímetro em série com o circuito.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/5-circuito-com-voltimetro-e-amperimetro.png?raw=true)

Além disso, cada resistor consome energia de acordo com o tempo. Para medir isso, basta usar a potência, em watts. (1W = 1 J/s)

    Potência no resistor: P = U ∙ i

Para identificar quanto vale a resistência de um resistor segundo as faixas de cores que estão nele, basta utilizar a seguinte tabela:

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/6-tabela-de-cores-de-resistores.png?raw=true)

### Capacitor

O capacitor é um componente que armazena cargas elétricas.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/7-capacitor-eletrolitico.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/8-funcionamento-do-capacitor.png?raw=true)
![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/9-possiveis-simbolos-de-capacitores.png?raw=true)

*Observação: Alguns tipos de capacitores são polarizados e outros não*

Em um capacitor, há um material isolante elétrico entre duas placas condutoras. Ao ligar o capacitor em um gerador de tensão, os elétrons se acumularão em uma das placas, gerando uma diferença de potencial entre seus terminais.

Em determinado momento, a diferença de potencial no capacitor será quase igual à diferença de potencial no gerador de tensão, e então o capacitor será carregado muito lentamente.

Uma vez carregado, o capacitor serve de gerador de tensão e pode ser descarregado em um circuito.

Para medir a capacidade de armazenamento de um capacitor, utiliza-se a grandeza escalar “capacitância”. Quanto maior a capacitância, maior a capacidade de armazenamento. A capacitância C (em farads) está associada com a área das placas condutoras S (em metros quadrados), a distância entre elas d (em metros) e a constante dielétrica ε (em farads por metro) pela seguinte relação:

    C = ε S/d

Há também outro jeito de calcular a capacitância:

    C = q/ΔV

Em que C é a capacitância, em farads, q é a carga elétrica armazenada, em coulombs, e V é a diferença de potencial, em volts.

Sendo assim, temos que 1F = 1C/V.

Ao associar capacitores em série ou paralelo, podemos obter um capacitor com capacitância equivalente aplicando as seguintes fórmulas:

    Associação em série: 1/Ceq = 1/C1 + 1/C2 + ⋯

    Associação em paralelo: Ceq = C1 + C2 + ⋯

É importante também estudar o circuito RC. (Resistor e Capacitor)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/10-circuito-rc.png?raw=true)

Nesse circuito, o capacitor levará um tempo para ser carregado. Estes gráficos descrevem o que acontece no circuito RC.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/11-graficos-circuito-rc.png?raw=true)

Vc é a tensão no capacitor, Qc é a carga no capacitor, Vr é a tensão no resistor e I é a corrente no circuito. (o resistor e o capacitor estão em série e a mesma corrente passa por eles)

Nesse circuito, o tempo que leva para o capacitor carregar é diretamente proporcional à capacitância e à resistência. (quanto maior a resistência/capacitância, maior o tempo que leva)

A tensão elétrica no gerador de tensão define qual será a tensão máxima que o capacitor poderá atingir.

*Observação: Ao descarregar o capacitor em um resistor, os gráficos são semelhantes, mas a tensão e a carga no capacitor diminuem ao invés de aumentar.*

### Diodo

O diodo é um componente que só deixa passar corrente em um sentido.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/12-diodo.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/13-simbolo-diodo.png?raw=true)

O sentido que o diodo permite a corrente passar é o sentido da seta em seu símbolo.

Em um diodo real, se determina esse sentido através da faixa cinza que há nele. Chamamos o terminal mais próximo da faixa cinza de cátodo (negativo) e o terminal mais longe de ânodo (positivo).

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/14-diodo-anodo-catodo.png?raw=true)

Caso o diodo seja ligado diretamente (negativo no cátodo e positivo no ânodo), a corrente fluirá como se o diodo fosse uma chave fechada. Caso ele seja conectado inversamente (positivo no cátodo e negativo no ânodo), o diodo se comportará como uma chave aberta.

Na realidade, o diodo conectado diretamente funciona como chave fechada a partir de determinada tensão. Para entender melhor como isso funciona, veja a figura abaixo.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/15-diodo-polarizacao.png?raw=true)

A região do meio de um diodo é chamada de barreira de potencial (ou camada de depleção). Ela separa o cátodo e o ânodo de um diodo. Quando um diodo é ligado inversamente, essa barreira aumenta pois as cargas positivas são atraídas para o polo negativo da pilha e as cargas negativas, para o polo positivo da pilha. Já se o diodo é ligado diretamente, ao aumentar a tensão, a barreira de potencial fica cada vez menor até que, em certo momento, ela desaparece e o diodo passa a funcionar como um fio.

Dessa forma, o diodo causa uma queda de tensão no circuito. No exemplo abaixo, apesar da fonte de tensão fornecer 10V, a tensão no resistor será em torno de 9.2V, já que se trata de um diodo de silício (o material influencia na tensão necessária para "quebrar" a barreira de potencial).

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/16-circuito-e-grafico-diodo.png?raw=true)

*Observação: é comum dizer que o diodo de silício causa uma queda de tensão de aproximadamente 0.7V. Aqui neste documento está escrito como se causasse 0.8V por conta do gráfico presente na imagem*

O significado da sigla LED é *Light Emissor Diode*, ou seja, se trata de um diodo também. LEDs costumam causar uma queda de tensão maior que 0.7V, geralmente multímetros possuem uma função para calcular essa tensão.

### Diodo Zener

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/17-simbolo-diodo-zener.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/18-grafico-diodo-zener.png?raw=true)

O diodo zener é como um diodo normal, porem a partir de certa tensão ele passa a ser um curto circuito, essa é a TENSÃO ZENER. Se a tensão no diodo zener for menor que a tensão zener ele não conduz, assim como os diodos convencionais. Se a tensão for maior que a tensão zener, o diodo zener mesmo estando contrario ao circuito vai conduzir.

    Uin < |Vzener|, Uout = Uin

    Uin > |Vzener|, Uout = Vzener

O diodo zener tem uma corrente máxima suportável, e isso é delimitado de acrodo com a potencia do componente, caso a pontência do circuito seja ultrapassada, o diodo pode se danificar.

    Izmax = Pz/Vz

    Izmin = Izmax ∙ 0.10

    Rzmin = (Vcc - Vz)/Izmax

    Rzmax = (Vcc - Vz)/Izmin

*Rz: Resistor limitador de corrente*

Esse diodo é muito bom para retificar a onda de tensão, principalmente quando se deseja estabelecer uma tensão continua. Nesse ciruito, o zener pode ser útil, porque ele controla a tensão, cortando-a em apenas um valor. Isso acontece porque ele mantém o valor de tensão máxima em seus terminais caso esteja conduzindo reversamente.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/19-circuito-com-zener.png?raw=true)

Esse é um simples circuito limitador de tensão usando zener. Vout sempre será Vz (tensão zener) na carga sempre que Vin > Vz, já que o diodo zener irá limitar.

### Traformadores
O transformador modifica os níveis de tensão e corrente elétrica, mantendo a potência constante.
No projeto da fonte vamos precisar de um transformador para reduzir a tensão da tomada, 110V ou 220V, para uma tensão entre 3V - 12V.
Como a potência se mantém constante, ao usarmos o transformador para diminuir a tensão, a corrente do nosso circuito vai aumentar. 
P1 = P2 <=> V1*I1 = V2*I2

Estrutura:
Enrolamento:  O enrolamento de um transformador é formado de várias bobinas (os transformadores mais comuns usam duas) que em geral são feitas de cobre. Quando a corrente passa pela bobina forma um campo magnético que produz uma tensão elétrica nas extremidades desse enrolamento. A alteração na corrente presente na bobina do circuito primário altera o fluxo magnético nesse circuito e também na bobina do circuito secundário.

Núcleo: responsável por transferir a corrente do enrolamento primário para o enrolamento secundário. A mudança no fluxo magnético na bobina secundária induz uma tensão elétrica na bobina secundária

O transformador altera a tensão através de duas bobinas, seguindo uma proporção de uma bobina para a outra. ex: se tivermos 100 voltas em uma e 10 voltas na outra, a tensão será transformada na proporção de 10 para 1, ou seja, se tivermos 100V na entrada, teremos 10V na saída.


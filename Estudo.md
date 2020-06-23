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

Há coisas como corrente e tensão máximas que um diodo pode suportar. Isso depende do diodo e esse tipo de informação pode ser encontrada no datasheet.

### Diodo Zener

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/17-simbolo-diodo-zener.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/18-grafico-diodo-zener.png?raw=true)

O diodo zener é como um diodo normal, porem a partir de certa tensão ele passa a ser um curto circuito, essa é a TENSÃO ZENER. Se a tensão no diodo zener for menor que a tensão zener ele não conduz, assim como os diodos convencionais. Se a tensão for maior que a tensão zener, o diodo zener mesmo estando contrario ao circuito vai conduzir.

    Uin < |Vzener|, Uout = Uin

    Uin > |Vzener|, Uout = Vzener

O diodo zener tem uma corrente máxima suportável, e isso é delimitado de acordo com a potencia do componente, caso a potência do circuito seja ultrapassada, o diodo pode se danificar.

    Izmax = Pz/Vz

    Izmin = Izmax ∙ 0.10

    Rzmin = (Vcc - Vz)/Izmax

    Rzmax = (Vcc - Vz)/Izmin

*Rz: Resistor limitador de corrente*

Esse diodo é muito bom para retificar a onda de tensão, principalmente quando se deseja estabelecer uma tensão continua. Nesse ciruito, o zener pode ser útil, porque ele controla a tensão, cortando-a em apenas um valor. Isso acontece porque ele mantém o valor de tensão máxima em seus terminais caso esteja conduzindo reversamente.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/19-circuito-com-zener.png?raw=true)

Esse é um simples circuito limitador de tensão usando zener. Vout sempre será Vz (tensão zener) na carga sempre que Vin > Vz, já que o diodo zener irá limitar.

### Transformadores
O transformador modifica os níveis de tensão e corrente elétrica, mantendo a potência constante.
Como a potência se mantém constante, ao usarmos o transformador para diminuir a tensão, a corrente do nosso circuito vai aumentar.

    P1 = P2 <=> V1 . I1 = V2 . I2

Estrutura:
Enrolamento:  O enrolamento de um transformador é formado de várias bobinas (os transformadores mais comuns usam duas) que em geral são feitas de cobre. Quando a corrente passa pela bobina forma um campo magnético que produz uma tensão elétrica nas extremidades desse enrolamento. A alteração na corrente presente na bobina do circuito primário altera o fluxo magnético nesse circuito e também na bobina do circuito secundário.

Núcleo: responsável por transferir a corrente do enrolamento primário para o enrolamento secundário. A mudança no fluxo magnético na bobina secundária induz uma tensão elétrica na bobina secundária

O transformador altera a tensão através de duas bobinas, seguindo uma proporção de uma bobina para a outra. ex: se tivermos 100 voltas em uma e 10 voltas na outra, a tensão será transformada na proporção de 10 para 1, ou seja, se tivermos 100V na entrada, teremos 10V na saída.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/20-simbolo-transformador.png?raw=true)

*Observação: damos o nome de primário o enrolamento da esquerda e secundário o da direita*

Os valores analisados em um transformador são relativos à tensão eficaz. Por exemplo, a tensão eficaz V1 é transformada na tensão eficaz V2.
Para calcular a tensão eficaz, basta dividir a tensão de pico por √2.

As tomadas residenciais geralmente fornecem de 110V a 127V ou de 220V a 254V de tensão eficaz.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/21-tensao-eficaz.png?raw=true)

Há transformadores com derivação central. Segue na imagem abaixo um exemplo de um.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/22-transformador-derivacao-central.png?raw=true)

Se o transformador for 12V + 12V, por exemplo, significa que entre um dos terminais laterais e o terminal do meio, há 12V. Dessa forma, ao medir a tensão entre os terminais laterais, o resultado deve ser 24V (tensão eficaz)

Além disso, transformadores reais possuem rendimento, pois dissipam calor. Por exemplo, um transformador com 90% de rendimento, significa que a potência no secundário é 90% da potência no primário. Transformadores bons possuem mais que 90% de rendimento.

Geralmente transformadores são projetados também com um fio a mais no primário para tornar possível a escolha entre 127V ou 220V.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/23-transformador-12-12.png?raw=true)

Este é um exemplo de transformador real. Nesse caso, o fio de 127V está no meio da bobina, como na derivação central, mas não se encontra exatamente no meio.

Uma chave seletora pode ajudar na passagem de 127V para 220V e vice-versa.

### Potenciômetro

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/24-potenciometro-real.png?raw=true)

Um potenciômetro é como se fosse um conjunto de duas resistências em que é possível regular manualmente a proporção em que cada uma delas vai receber da resistência total. Segue duas imagens para melhor entendimento.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/25-potenciometro-funcionamento.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/26-potenciometro-analogia-resistores.png?raw=true)

O cursor pode ser ajustado manualmente. Ele determina qual porção da resistência total do potenciômetro o R1 e o R2 vão ter. Note que R1 + R2 deve ser igual à resistência do potenciômetro.

Note também que tc é o terminal do cursor, enquanto t1 e t2 são os terminais de R1 e de R2, respectivamente.

Suponha um potenciômetro de 100Ω. R1 + R2 sempre será 100Ω, mas o valor de R1 e de R2 pode ser regulado pelo cursor. Por exemplo, ao aproximar o cursor de t1, R1 se aproxima de 0Ω e R2 se aproxima de 100Ω. Ao aproximar de t2, R2 se aproxima de 0Ω enquanto R1 se aproxima de 100Ω. Há infinitos valores intermediários, como R1 = 67.3Ω e R2 = 32.7Ω.

Potenciômetros podem ser encontrados, por exemplo, em caixas de som no regulador de áudio.

### Transistor NPN

O transistor TBJ NPN, é um componente que funciona como uma válvula/interruptores de tensão em um circuito, ou também, ele funciona ou barrando, ou amplificando a corrente elétrica. Seu funcionamento depende de 3 terminais, base, coletor e emissor. A corrente a ser controlada é a Ic := corrente no coletor, ou seja, é a corrente que passa do coletor ao emissor.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/32-transistor-desenho-1.png?raw=true)

1) Base: é o terminal controlador, ele que determina se haverá ou não passagem de corrente entre o coletor e o emissor.

2) Coletor: entrada do transistor, ela que inicialmente controla a tensão e corrente no emissor.

3) Emissor: saída do transistor.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/33-transistor-desenho-2.png?raw=true)

Definição de Variáveis:

a) Vc: tensão no coletor;

b) Vb: tensão na base;

c) Vbe: tensão entre a base e o emissor, normalmente está entre 0,7V;

d) Ve: tensão no emissor;

Ve(max) = Vb – Vbe

Inicialmente, Ve = Vc; Mas caso, Vc < Vb: Ve = Vb – Vbe.

e) Vce = Vc – Ve;

f) Ie = Ve / Re;

g) Ic = Ie * a = Ie * ganho/ganho+1		ou	Ic = Ib * ganho

h) Ib = Ic / ganho		ou	Ib = (Vb – Vc ) / Rb

## Seções da fonte

### Papel do Transformador

No projeto da fonte vamos precisar de um transformador para reduzir a tensão da tomada, 110V ou 220V, para uma tensão entre 3V - 12V.

O papel do transformador na fonte é reduzir a tensão da entrada para que o circuito não precise trabalhar com tensões muito elevadas que podem danificar componentes ou exigir componentes mais caros.

### Papel da Ponte Retificadora

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/27-ponte-retificadora.png?raw=true)

A ponte retificadora, uma associação de 4 diodos, serve para transformar a corrente alternada em uma corrente contínua pulsante (a polaridade se mantém, mas a tensão ainda varia com o tempo). A propriedade dos diodos que é utilizada na ponte retificadora é a de não conduzir quando está polarizado inversamente.

Segue uma análise da ponte retificadora em uma carga.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/28-ponte-retificadora-sentido-1.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/29-ponte-retificadora-sentido-2.png?raw=true)

Note que tanto faz se o positivo está em cima e o negativo em baixo, ou o positivo em baixo e o negativo em cima. A corrente fluirá pela carga R1 no mesmo sentido: cima para baixo.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/30-ponte-retificadora-grafico.png?raw=true)

A corrente alternada passa pela ponte retificadora e se torna corrente contínua pulsante.

### Papel do Capacitor

O papel do capacitor na fonte é proporcionar o *ripple*. Como agora a corrente é contínua e pulsante, o capacitor armazena a carga e descarrega lentamente enquanto a tensão estaria abaixo da tensão que o capacitor obteve. Segue um gráfico para entender melhor o que seria o *ripple*.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/31-ripple.png?raw=true)

No começo do primeiro ciclo da onda, o capacitor estará sendo carregado até a tensão de pico. Quando a tensão cai, o capacitor libera a carga que foi armazenada aos poucos, até que a tensão de do segundo ciclo da onda seja maior que a tensão no capacitor, que irá carregá-lo novamente. Isso se segue repetidas vezes.

Com o *ripple*, a tensão está mais estável: ainda varia, mas muito menos.

### Papel do Diodo Zener

Antes de mais nada, deve-se entender o que é um divisor de tensão.

#### Divisor de tensão

O divisor de tensão nada mais é que uma análise da tensão em um resistor de um circuito de vários resistores associados em série.

O caso mais comum é o de dois resistores conectados em série. Nesse caso, a fórmula para calcular a tensão no resistor R2 é a seguinte:

    (V ∙ R2) / (R1 + R2)

Em que V é a tensão da alimentação.

A fórmula para R1 é análoga, e para divisores de tensão com mais resistores, basta considerar como R1 (ou R2) o resistor equivalente à todos os resistores exceto aquele cuja tensão está sendo analisada.

O divisor de tensão é uma consequência direta da lei das malhas de *Kirchhoff*.

#### Divisor de tensão combinado com diodo zener

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/19-circuito-com-zener.png?raw=true)

Basicamente, o circuito do divisor de tensão junto com o zener é este.

Funciona da seguinte forma: se o Vout calculado pelo divisor de tensão em Rl for menos que o Vzener, então a tensão em Rl (e no zener) será Vout e a tensão em Rs será Vin - Vout.

Mas se Vout for maior que Vzener, a tensão em Rl e no zener será Vzener, e a tensão em Rs será Vin - Vzener.

Observe que o diodo zener está polarizado inversamente. Apenas dessa forma o circuito funcionará do modo esperado.


#### Papel na fonte

Necessário estudar o transistor NPN antes de prosseguir.

## Dimensionamento

### Transformador

Transformador utilizado: 10+10 bivolt 800mA. Usaremos os terminais das pontas a fim de obter 20V

https://produto.mercadolivre.com.br/MLB-1304934993-transformador-trafo-1010v-800ma-bivolt-eletrnica-_JM?matt_tool=82322591&matt_word&gclid=CjwKCAjwxLH3BRApEiwAqX9are-Hoqy3DhheSooU8NO5g_m_VOuyIxmSU64KT07Ga4GBR1CclxpqFRoCT10QAvD_BwE&quantity=1

Preço: 30 reais

Dados no circuito: a tensão máxima no secundário será de aproximadamente 28,28V. A corrente que passará por ele será de x mA

Por que usaremos esse transformador:

### Diodos para ponte retificadora

Diodos utilizados: 1n4001.

https://www.robocore.net/loja/itens-eletronicos/diodo-1n4007?gclid=CjwKCAjwxLH3BRApEiwAqX9arQYP_1w9nsWFqdvp4X-WlUcxEd8-nIBf6EI5o0YcvvptZfaJRTloMRoCyW0QAvD_BwE

Preço: 18 centavos a unidade

Dados no circuito: provocará uma queda de tensão de 0,7V cada um. A tensão máxima que antes era 28,28V, será de 26,88V depois de passar pela ponte retificadora.

Por que usaremos esse diodo: pois ele é comum, barato e suporta até 50V

### Capacitor

Capacitor utilizado: eletrolítico 470uF / 50V

https://www.baudaeletronica.com.br/capacitor-eletrolitico-470uf-50v.html

Preço: 82 centavos

Dados no circuito: proporcionará um ripple de 25,1V a 26,88V

Por que usaremos esse capacitor: é comum, barato, torna a variação de tensão no ripple baixa e suporta até 50V.

### Diodo Zener

Zener utilizado: BZX55C [13V / 0.5W]

https://www.baudaeletronica.com.br/diodo-zener-bzx55c-13v-0-5w.html

Preço: 8 centavos

Dados no circuito: a corrente que passará por ele será de 15 mA (o circuito foi dimensionado pensando nessa corrente).

Por que usaremos esse zener: é comum, barato e como o circuito será regulado a no maximo 12V e há uma queda de tensão entre base e emissor no transistor, 13V é o ideal.

### Transistor NPN

Transistor NPN utilizado: BC337

https://www.robocore.net/loja/itens-eletronicos/transistor-npn-bc337?gclid=CjwKCAjwxLH3BRApEiwAqX9arW03jdNyoyxCW0BkSUH1jNxcEZlj1NO8uKe5adsfmaa_ggKm3B1-3hoC9gwQAvD_BwE

Preço: 24 centavos a unidade

Dados no circuito: os dados irão depender de como o potenciômetro será regulado e da resistência na carga

Considerando uma carga de 120 ohm e o potenciômetro no estado em que o máximo de tensão é fornecida à carga, como há uma queda de tensão de 0,7V, a carga receberá em torno de 12,3V no máximo, então a corrente no emissor será de 102,5 mA

Considerando o ganho mínimo de 100, a corrente na base será 1,01mA, e no coletor será 101,5mA

Considerando agora o ganho máximo de 630, a corrente na base será 0,16mA, e no coletor será 102,34mA

A tensão de base e coletor será entre 12,1V e 13,88V

Por que usaremos esse transistor: é comum, barato e suporta a tensão e corrente necessárias no circuito

### Resistências e potenciômetro no regulador

Resistências utilizadas:

Potenciômetro utilizado:

Preço:

Dados no circuito: as resistências e o potenciômetro foram dimensionados de forma a cumprir aproximadamente todos os requisitos abaixo

    Vin * (R2 + Rp)/(R2 + Rp + R1) > 13V

    i1 = 15mA + i2

    i2 = 1,05mA + i3

    Rp = 2,5 R2

    i1 < 30mA

Para obter valores com folga e disponíveis para compra:

    Vin = 26 (está entre 25,1 e 26,88)

Tomando Rp = 5k

    R2 = 2k

    i3 = 1,86mA

    i2 = 2,86mA

    i1 = 17,86mA

    R1 = 750ohm

    V1 * (R2 + Rp)/(R2 + Rp + R1) = 26 * 7000/7750 = 23,5V > 13V

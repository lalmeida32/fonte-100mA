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

Sendo assim, temos que
    1F = 1C/V.

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

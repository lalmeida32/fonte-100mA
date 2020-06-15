# Estudo do Projeto

Fonte de 100mA

## Introdução

Neste documento se encontram as informações adquiridas para a montagem da fonte.

## Componentes

### Resistor

O resistor é um dispositivo elétrico que consome corrente elétrica. É utilizado principalmente para limitar a corrente elétrica em um circuito e para converter energia elétrica em energia térmica.

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/1-resistor.png?raw=true)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/estudo-do-projeto/images/2-simbolo-resistor.png?raw=true)

Uma equação importante ao trabalhar com resistores é U=R∙i (Primeira Lei de Ohm), em que U é a diferença de potencial (em Volts), R é a resistência (em Ohms) e i é a corrente elétrica (em Amperes). A corrente no circuito varia de acordo com a resistência e a tensão.

    Primeira Lei de Ohm: U = R ∙ i

Outra equação importante para entender a grandeza “resistência elétrica”, é a Segunda Lei de Ohm. Na verdade, até um fio apresenta resistência, mas em circuitos simples não é necessário considerá-la.

    Segunda Lei de Ohm: R = (ρ ∙ L)/A

Nesse caso, ρ é uma constante associada ao material, (resistividade do material) L é o comprimento do fio e A é a área da seção transversal do fio.

Resistores combinados em série e em paralelo podem ser substituídos por um resistor equivalente. Caso os resistores sejam ligados em série, a nova resistência será igual à soma das resistências. Em paralelo, o inverso da nova resistência será igual à soma do inverso das resistências.

    Associação em série: Req = R1+R2+⋯

    Associação em paralelo: 1/Req =1/R1 +1/R2 +⋯

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

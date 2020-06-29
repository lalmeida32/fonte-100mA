# Dimensionamento

##

## Link para o Circuito

###

### tinyurl.com/y8z7htxh

##

## Transformador

Transformador utilizado: 10+10 bivolt 800mA. Usaremos os terminais das pontas a fim de obter 20V

https://produto.mercadolivre.com.br/MLB-1304934993-transformador-trafo-1010v-800ma-bivolt-eletrnica-_JM?matt_tool=82322591&matt_word&gclid=CjwKCAjwxLH3BRApEiwAqX9are-Hoqy3DhheSooU8NO5g_m_VOuyIxmSU64KT07Ga4GBR1CclxpqFRoCT10QAvD_BwE&quantity=1

Preço: 30 reais

Dados no circuito: a tensão máxima no secundário será de aproximadamente 28,28V.

Por que usaremos esse transformador: Atende às necessidades, já que a tensão fornecida será maior que 13V com folga, é barato e não será  danificado pela corrente que passará por ele.

##

## Diodos para ponte retificadora

Diodos utilizados: 1n4007

https://www.robocore.net/loja/itens-eletronicos/diodo-1n4007?gclid=CjwKCAjwxLH3BRApEiwAqX9arQYP_1w9nsWFqdvp4X-WlUcxEd8-nIBf6EI5o0YcvvptZfaJRTloMRoCyW0QAvD_BwE

Preço: 18 centavos a unidade

Dados no circuito: provocará uma queda de tensão de 0,7V cada um. A  tensão máxima que antes era 28,28V, será de 26,88V depois de passar pela ponte retificadora.

Por que usaremos esse diodo: pois ele é comum, barato e suporta alta  tensão (um 1n4001 seria suficiente, mas na internet foi mais fácil  encontrar 1n4007).

##

## Capacitor

Capacitor utilizado: eletrolítico 270uF / 50V

https://produto.mercadolivre.com.br/MLB-1539705638-cap-eletrolitico-270uf-50v-kit-c-50-pcs-_JM?matt_tool=79246729&matt_word&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgJOoLrQkDYLJqg39wcG0bboEYxBCcrLzJXZ2tlZwHFAX_THqohX_jQaArT6EALw_wcB&quantity=1

Preço: 31 centavos a unidade

Dados no circuito: proporcionará um ripple de 23,9V a 26,88V

Por que usaremos esse capacitor: é comum, barato, torna a variação de tensão no ripple baixa e suporta até 50V.

##

## Diodo Zener

Zener utilizado: BZX55C [13V / 0,5W]

https://www.baudaeletronica.com.br/diodo-zener-bzx55c-13v-0-5w.html

Preço: 9 centavos

Dados no circuito: a corrente que passará por ele será de 8,2 mA a 10,9 mA, aproximadamente (a variação ocorre por conta do *ripple*). Para que o diodo funcione corretamente, é necessário que passe ao menos 3,8mA por ele (e no máximo, 38mA). Dessa forma, ele está sendo  alimentado de maneira correta: com folga e sem danificá-lo.

Por que usaremos esse zener: é comum, barato, e como o circuito será  regulado a no máximo 12V e há uma queda de tensão entre base e emissor  no transistor, 13V é o ideal.

##

## Transistor NPN

Transistor NPN utilizado: BC337

https://www.robocore.net/loja/itens-eletronicos/transistor-npn-bc337?gclid=CjwKCAjwxLH3BRApEiwAqX9arW03jdNyoyxCW0BkSUH1jNxcEZlj1NO8uKe5adsfmaa_ggKm3B1-3hoC9gwQAvD_BwE

Preço: 24 centavos a unidade

Dados no circuito: os dados irão depender de como o potenciômetro será regulado e da resistência na carga

Considerando uma carga de 120 ohm e o potenciômetro no estado em que o máximo de tensão é fornecida à carga, como há uma queda de tensão de  0,7V, a carga receberá em torno de 12,3V no máximo, então a corrente no  emissor será de 102,5 mA

```
Considerando o ganho mínimo de 100, a corrente na base será 1,01mA, e no coletor será 101,5mA

Considerando agora o ganho máximo de 630, a corrente na base será 0,16mA, e no coletor será 102,34mA

A tensão entre base e coletor será entre 10,9V e 13,88V.
```

Quando o potenciômetro estiver no estado em que o mínimo de tensão é  fornecida à carga, a corrente será desprezível e a tensão entre base e  coletor será entre 20,2V e 23,18V.

Por que usaremos esse transistor: é comum, barato e suporta a tensão e corrente necessárias no circuito

##

## Resistores e potenciômetro no regulador

Resistores utilizados: 1k e 2.2k

Potenciômetro utilizado: 5k

https://www.engetronic-sc.com.br/produtos/ver/321/potenciometro-linear-5k-l15---eixo-estriado-tracking-google-shopping?gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgJ0FChjyK9vocYBgfldQy7j2Pse0-l_idTZ0iNpJngsEBgyiqvtofkaAqLBEALw_wcB

https://www.robocore.net/loja/itens-eletronicos/resistor-1k-pacote-com-10-unidades?gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgIWM1y2G34SD7-tczS923PPDzohgqbYDrJMymhz6VmJgYpguPpxyvwaAvVsEALw_wcB

https://www.eletroinfocia.com.br/resistor-1-4w-2k2?parceiro=5383&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgIYW0y8DoWLAFSC3mD8_5y1W9r2wVgBxpERvJd_8GI4131PIfijfdAaArM8EALw_wcB

Preço: por volta de 2 reais e 10 centavos

Dados no circuito:

Tomando Rp = 5k, R2 = 2.2k e R1 = 1k e considerando o caso em que o potenciômetro está fornecendo o máximo de tensão à carga.

Primeiro, considerando o menor valor para Vin possível (23,9V):

```
Corrente no resistor R1: 10,9mA

Corrente no resistor R2: 1,8mA

Vin * (R2 + Rp)/(R2 + Rp + R1) = 23,9 * 7200/8200 = 21V > 13V
```

Agora, o maior valor possível (26,88V):

```
Corrente no resistor R1: 13,9mA

Corrente no resistor R2: 1,8mA

26,88 * 7200/8200 > 21V > 13V
```

Por que usaremos esses resistores e esse potenciômetro: são fáceis de encontrar (valores comerciais), baratos, suportam a corrente que  passará por eles com folga e atendem às necessidades do circuito.

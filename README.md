# Projeto: Fonte-100mA — TRABALHO 01







### Grupo 19, Integrantes:

* Adrio O. Alves (*11796830*)
* Eduardo V. B. Rossi (*10716887*)
* Felipi Y. Santos (*11917292*)
* Lucas F. de Almeida (*1162063*)



**Docente**: Eduardo do Valle Simões
**Curso**: SSC0180 - Eletrônica para Computação





**Bacharelado em Ciências da Computação — 2020**
**Instituto de Ciências Matemáticas e de Computação**
**Universidade de São Paulo**

---









# Introdução



​	O projeto de trabalho 1 tem como objetivo a construção de uma fonte de alimentação genérica que precisa  fornecer corrente de até 100mA (*miliampères*) e uma tensão entre 3V e 12V. O projeto conta com um diagrama contendo os componentes eletrônicos escolhidos para construção da fonte, juntamente com o preço de cada um. Além disso, o projeto da fonte foi modelado em duas ferramentas de construção de circuitos: Falstad e EAGLE, e também um vídeo apresentando uma visão geral.







 # O repositório



* **estudo-do-projeto**

  * *Estudos.md*: Esse markdown dá informações do que cada componente eletrônico usado na fonte é, como ele é usado na fonte, isto é, seu papel.

  * **imagens**: fotos de peças/dependência do Estudos.md

  * *Dimensionamento.md*: relação de gastos e links para cada componente



* **arquivos-circuitos**

  * **FONTE**: arquivos do projeto no Eagle (contém esquemático e PCB)
  * *circuit-20200628-2337.circuitjs.txt*: um export do circuito feito no Falstad.
  * **EAGLE:** diretório contendo os arquivos do projeto no EAGLE
  * *eagle.jpg*: um export do projeto esquemático no EAGLE
  * *pcb.png*: um export do projeto em PCB no EAGLE
  * *circuito.png*: foto do circuito no falstad



# Diagrama da Fonte

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/revisao-do-projeto/arquivos-circuitos/circuito.png?raw=true)

![img](https://i.imgur.com/2E5dJVi.jpg)

![alt text](https://github.com/cs-lucasalmeida/fonte-100mA/blob/revisao-do-projeto/arquivos-circuitos/pcb.png?raw=true)







# Relação componente/valores



**Obs**.: Desconsideramos o frete pois os preços de entrega encontram-se mais elevados durante o período da Pandemia (COVID-19). 



| Componente                                         | Links                                                        | Quantidade | Preço resultante           |
| -------------------------------------------------- | ------------------------------------------------------------ | ---------- | -------------------------- |
| **Transformador**               10+10 bivolt 800mA | https://produto.mercadolivre.com.br/MLB-1304934993-transformador-trafo-1010v-800ma-bivolt-eletrnica-_JM?matt_tool=82322591&matt_word&gclid=CjwKCAjwxLH3BRApEiwAqX9are-Hoqy3DhheSooU8NO5g_m_VOuyIxmSU64KT07Ga4GBR1CclxpqFRoCT10QAvD_BwE&quantity=1 | x1         | R$ 30,00                   |
| **Diodos da ponte retificadora** (1n4007)          | https://www.robocore.net/loja/itens-eletronicos/diodo-1n4007?gclid=CjwKCAjwxLH3BRApEiwAqX9arQYP_1w9nsWFqdvp4X-WlUcxEd8-nIBf6EI5o0YcvvptZfaJRTloMRoCyW0QAvD_BwE | x4         | R$ 0,18        x 4 =  0,72 |
| **Capacitor** eletrolítico 270uF / 50V             | https://produto.mercadolivre.com.br/MLB-1539705638-cap-eletrolitico-270uf-50v-kit-c-50-pcs-_JM?matt_tool=79246729&matt_word&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgJOoLrQkDYLJqg39wcG0bboEYxBCcrLzJXZ2tlZwHFAX_THqohX_jQaArT6EALw_wcB&quantity=1 | x1         | R$ 15,50                   |
| **Diodo Zener** (BZX55C 13V/0,5W)                  | https://www.baudaeletronica.com.br/diodo-zener-bzx55c-13v-0-5w.html | x1         | R$ 0,09                    |
| **Transistor NPN** (BC337)                         | https://www.robocore.net/loja/itens-eletronicos/transistor-npn-bc337?gclid=CjwKCAjwxLH3BRApEiwAqX9arW03jdNyoyxCW0BkSUH1jNxcEZlj1NO8uKe5adsfmaa_ggKm3B1-3hoC9gwQAvD_BwE | x1         | R$ 1,20                    |
| **Resistor** (1kΩ)                                 | https://www.robocore.net/loja/itens-eletronicos/resistor-1k-pacote-com-10-unidades?gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgIWM1y2G34SD7-tczS923PPDzohgqbYDrJMymhz6VmJgYpguPpxyvwaAvVsEALw_wcB | x1         | R$ 0,75                    |
| **Resistor** (2.2kΩ)                               | https://www.eletroinfocia.com.br/resistor-1-4w-2k2?parceiro=5383&gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgIYW0y8DoWLAFSC3mD8_5y1W9r2wVgBxpERvJd_8GI4131PIfijfdAaArM8EALw_wcB | x1         | R$ 0,10                    |
| **Potenciômetro**                                  | https://www.engetronic-sc.com.br/produtos/ver/321/potenciometro-linear-5k-l15---eixo-estriado-tracking-google-shopping?gclid=Cj0KCQjw3Nv3BRC8ARIsAPh8hgJ0FChjyK9vocYBgfldQy7j2Pse0-l_idTZ0iNpJngsEBgyiqvtofkaAqLBEALw_wcB | x1         | R$ 1,35                    |
| **TOTAL:**                                         |                                                              | 11         | R$ 49,72                   |









# Sobre os componentes não encontrados no EAGLE



​	Como o EAGLE não possui todos os componentes que foram utilizados na fonte, tivemos de utilizar componentes com funcionalidade e dimensões iguais no lugar.






# Links

* Vídeo explicativo da fonte: https://youtu.be/iQQ3Y2TPxfM
* Falstad (cópia em arquivos-circuitos): https://tinyurl.com/y8z7htxh
* Eagle (esquemático): https://imgur.com/a/H5OCaSa
* Eagle (PCB): https://imgur.com/a/zWWUykP

# Projeto do Subsistema de Energia
O subsistema de energia é responsável pela alimentação dos demais subsistemas, garantindo eficiência energética e capacidade de operação. Portanto, o foco da equipe consistiu em dimensionar os gastos energéticos, selecionar componentes eficazes, de baixo consumo e implementar estratégias de gerenciamento de energia em conformidade com as normas de segurança aplicáveis, assegurando a proteção dos usuários e a conformidade com os padrões de qualidade e regulamentações pertinentes.

## Levantamento de carga
Com o intuito de determinar a quantidade total de energia que será consumida no projeto realizou-se uma análise do consumo estimado dos dispositivos. Nessa análise será estimado um tempo de operação de leitura dos objetos de  30  minutos, um tempo mais preciso será somente possível na fase de testes. Para uma margem de segurança foi adicionado  20%  sobre o consumo do projeto. Assim, temos o consumo energético do projeto:

| Componente | Qtd | Corrente [A]|Tensão [V] |Tempo de Operação [h] |Potência [Wh]|
| ------ | ------ |------ |------ |------ |------ |
|ARDUINO UNO|1|0,41|5,00|0,50|1,03|
|L298N (PONTE H)|2|2,00|12,00|0,50|24,00|
|Potência Total [Wh]|||||25,03|
|Potência Total com 20% [Wh]|||||30,03|

## Bateria
Para o projeto ScanPoint está estimado em utilizar duas baterias de  12 V  com uma capacidade de 7AH cada, caso haja a necessidade de uma maior autonomia no projeto será adicionado mais uma bateria com as mesmas característica, mas em uma configuração em paralelo, visto que na configuração em série aumentaria a tensão e não é o que se deseja visto que os componentes do projeto apresentam uma tensão de alimentação inferior a 12V.

![Bateria](../assets/eletronica-energia/bateria_unipower.jpg)

| Marca                             | UNICOBA       |
|------                             | ------        |
|    Modelo                         |UP 1270 SEG      |
|Composição das células da bateria  |Chumbo - Ácido |
|Voltagem                           | 12V            |
|    Amperagem                      |    7Ah        |
|    Dimensões [cm]                 |   8x16x11    |
|    Peso[kg]                       |    2,00        |

## Cabo
A corrente elétrica solicitada pelo sistema é de  2,41A. A NBR  5410  será consultada a fim de levar em consideração alguns fatores para o dimensionamento dos cabos elétricos.

![Tabela33](../assets/eletronica-energia/Tabela33.jpg)

**Fonte: NBR 2410, 2004**

Ao consultar a Tabela  33  da norma será considerado o Método de referência  B1 .

![Tabela40](../assets/eletronica-energia/Tabela40.jpg)

**Fonte: NBR 2410, 2004**

Ao analisar a Tabela  40  será considerado uma temperatura ambiente de  25°C , visto que segundo o site do Instituto Nacional de Meteorologia (INMET) as temperaturas no Distrito Federal para o mês de julho ficam entre  20°C  e  25°C . Logo, para uma isolação de PVC seu fator de correção será de  1,06 .

![Tabela42](../assets/eletronica-energia/Tabela42.jpg)

**Fonte: NBR 2410, 2004**

Ao analisar a Tabela  42  da norma será considerado  1  para o número de circuitos e como o método será o  B1 , logo, o fator será  1 .

Após a determinação dos fatores diante de um cenário que o projeto se encontrará, será feito os cálculos para corrigir a corrente elétrica em função desses fatores.

 I_{corrigida}=\frac{I_{sistema}}{F_{temperatura}×F_{agrupameto}}  [I]

Onde:

 I_{corrigida} : corrente elétrica corrigida;

 I_{sistema} : corrente elétrica do sistema;

 F_{temperatura} : fator de temperatura ambiente;

 F_{agrupamento} : fator de agrupamento do circuito.

Substituídos em [I] os valores determinados anteriormente:

 I_{corrigida} = \frac{2,41}{(0,87×1)}=2,77 A                [II]

Assim, tem-se uma corrente corrigida de  2,77 A . Será analisado a Tabela  37  a fim de determinar o cabo mais especificado para a corrente elétrica corrigida.


![Tabela37](../assets/eletronica-energia/Tabela37.jpg)

**Fonte: NBR 2410, 2004**

Baseado na corrente corrigida de  2,77 A  uma seção nominal de  0,5 mm^2  serviria, entretanto, a própria norma determina que para circuitos de força a seção nominal mínima deva ser de  2,5 mm^2 . Assim sendo, a seção nominal selecionada será a de  2,5 mm^2 .
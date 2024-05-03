# Projeto do Subsistema de Energia
<p style="text-alighn: justify;">
O subsistema de energia é responsável pela alimentação dos demais subsistemas, garantindo eficiência energética e capacidade de operação. Portanto, o foco da equipe consistiu em dimensionar os gastos energéticos, selecionar componentes eficazes, de baixo consumo e implementar estratégias de gerenciamento de energia em conformidade com as normas de segurança aplicáveis, assegurando a proteção dos usuários e a conformidade com os padrões de qualidade e regulamentações pertinentes.
</p>

## Levantamento de carga
<p style="text-alighn: justify;">
Com o intuito de determinar as características energéticas do projeto realizou-se uma análise do consumo estimado dos dispositivos. Para uma margem de segurança foi adicionado  20%  sobre a potência total do projeto.
</p>

Tabela 1: Levantamento de carga.

| Componente | Qtd | Corrente [A]|Tensão [V] |Potência [W]|
| ------ | ------ |------ |------ |------ |
|ARDUINO UNO|1|0,41|5,00|2,05|
|L298N (PONTE H)|2|2,00|12,00|48,00|
|Potência Total [W]||||50,05|
|Potência Total com 20% [W]||||60,06|




## Bateria
<p style="text-alighn: justify;">
Para o projeto ScanPoint está estimado em utilizar duas baterias de  12 V de 7Ah, cada.
</p>

![Bateria](../assets/eletronica-energia/bateria_unipower.jpg)

Figura 1 - Bateria UP1270SEG


Tabela 2 - Caracteríticas da bateria
| Marca                             | UNICOBA       |
|------                             | ------        |
|    Modelo                         |UP 1270 SEG      |
|Composição das células da bateria  |Chumbo - Ácido |
|Voltagem                           | 12V            |
|    Amperagem                      |    7Ah        |
|    Dimensões [cm]                 |   8x16x11    |
|    Peso[kg]                       |    2,00        |

<p style="text-alighn: justify;">
Nesse cenário o projeto apresenta uma autonomia de 2 horas e 48 minutos. Devido ao fato de não se ter o conhecimento real da leitura das peças não é possível determinar se o tempo de autonomia é suficiente ou não, assim,  caso haja a necessidade de uma maior autonomia no projeto, será adicionado baterias com as mesmas característica a fim de atender o tempo estipulado para a apresentação.
As baterias estarão configuradas em paralelo, visto que na configuração em série aumentaria a tensão, o que não é o desejado, pois os componentes do projeto apresentam uma tensão de alimentação inferior a 12V.
</p>


## Cabo
<p style="text-alighn: justify;">
A corrente elétrica solicitada pelo sistema é de  2,41A. A NBR  5410  será consultada a fim de levar em consideração alguns fatores para o dimensionamento dos cabos elétricos.
</p>

![Tabela33](../assets/eletronica-energia/Tabela33.jpg)

Figura 2 - Tipos de linhas elétricas. <font size="2"><p style="text-align: center">Fonte: [NBR 2410, 2004](https://edisciplinas.usp.br/pluginfile.php/5810747/mod_resource/content/1/NBR5410%20-%20Instala%C3%A7%C3%B5es%20el%C3%A9tricas%20de%20baixa%20tens%C3%A3o.pdf).</p></font>

Ao consultar a Figura 2 será considerado o Método de referência  B1 .

![Tabela40](../assets/eletronica-energia/Tabela40.jpg)

Figura 3 - Fatores de correção para a temperatura. <font size="2"><p style="text-align: center">Fonte: [NBR 2410, 2004](https://edisciplinas.usp.br/pluginfile.php/5810747/mod_resource/content/1/NBR5410%20-%20Instala%C3%A7%C3%B5es%20el%C3%A9tricas%20de%20baixa%20tens%C3%A3o.pdf).</p></font>

<p style="text-alighn: justify;">
Ao analisar a Figura 3  será considerado uma temperatura ambiente de  25°C , visto que segundo o site do Instituto Nacional de Meteorologia (INMET) as temperaturas no Distrito Federal para o mês de julho apresentam ma média que varia entre  20°C  e  25°C . Logo, para uma isolação de PVC seu fator de correção será de  1,06 .
</p>

![Tabela42](../assets/eletronica-energia/Tabela42.jpg)

Figura 4 - Fatores de correção aplicáveis a condutores. <font size="2"><p style="text-align: center">Fonte: [NBR 2410, 2004](https://edisciplinas.usp.br/pluginfile.php/5810747/mod_resource/content/1/NBR5410%20-%20Instala%C3%A7%C3%B5es%20el%C3%A9tricas%20de%20baixa%20tens%C3%A3o.pdf).</p></font>

<p style="text-alighn: justify;">
Ao analisar a Figura 4 da norma será considerado  1  para o número de circuitos e como o método será o  B1 , logo, o fator será  1 .
</p>

<p style="text-alighn: justify;">
Após a determinação dos fatores diante de um cenário que o projeto se encontrará, será feito os cálculos para corrigir a corrente elétrica em função desses fatores.
</p>

 $I_{corrigida}=\frac{I_{sistema}}{F_{temperatura}×F_{agrupameto}}  [I]$

Onde:

 $I_{corrigida} : corrente elétrica corrigida;$

 $I_{sistema} : corrente elétrica do sistema;$

 $F_{temperatura} : fator de temperatura ambiente;$

 $F_{agrupamento} : fator de agrupamento do circuito.$

Substituídos em [I] os valores determinados anteriormente:

 $I_{corrigida} = \frac{2,41}{(0,87×1)}=2,77 A              [II]$

<p style="text-alighn: justify;">
Assim, tem-se uma corrente corrigida de  2,77 A . Será analisado a Figura 5  a fim de determinar o cabo mais especificado para a corrente elétrica corrigida.
</p>


![Tabela37](../assets/eletronica-energia/Tabela37.jpg)

Figura 5 - Capacidade de condução de corrente. <font size="2"><p style="text-align: center">Fonte: [NBR 2410, 2004](https://edisciplinas.usp.br/pluginfile.php/5810747/mod_resource/content/1/NBR5410%20-%20Instala%C3%A7%C3%B5es%20el%C3%A9tricas%20de%20baixa%20tens%C3%A3o.pdf).</p></font>

<p style="text-alighn: justify;">
Baseado na corrente corrigida de  2,77 A  uma seção nominal de 0,5 mm^2 serviria, entretanto, a própria norma determina que para circuitos de força a seção nominal mínima deva ser de  2,5 mm^2 . Assim sendo, a seção nominal selecionada será a de 2,5 mm^2.
</p>

## Diagrama Unifilar

<p style="text-alighn: justify;">
A Figura 6 apresenta o diagrama unifilar do projeto, com as características de fluxo de energia, no qual cada componente está identificado com suas respectivas características elétrica, como também as características da bitola do cabo.
</p>

![Dia_Unifilar](docs/assets/eletronica-energia/Diagrama_unifilar_page-0001.jpg)

Figura 6 - Diagrama unifilar.


## Referências Bibliográficas

[1] Associação Brasileira de Normas Técnicas (ABNT). NBR 5410: Instalações elétricas de baixa tensão. Rio de Janeiro, 2004.

<div id="ref-2"/>
[2] Instituto Nacional de Meteorologia (INMET):: Clima. Prognóstico de Tempo (2024). Acesso em: 27 abr. 2024. Disponível em: https://clima.inmet.gov.br/progt.

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 28/04/2024 | Criação do documento | Lucas Pantoja |
| 1.1 | 29/04/2024 | Edição de textos, tabelas e imagens | Lucas Pantoja |
| 1.2 | 01/05/2024 | Modificação da tebela 1 | Lucas Pantoja |
| 1.3 | 03/05/2024 | Modificação de texto para padronização | Lucas Pantoja |

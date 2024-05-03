## Dados do projeto Nome do Projeto: Mesa giratória para impressão em 3D
Data de abertura: _/03/2024
Código: 1-A
Patrocinador: Universidade de Brasília 
Gerente: 

## Objetivos 
O presente projeto, intitulado “Mesa giratória para impressão em 3D”, encontrasse inserido no âmbito da disciplina de Projeto Integrador 2 e tem como objetivo a aplicação dos conhecimentos adquiridos nas áreas de engenharia aeroespacial, automotiva, software, eletrônica e energia. A relevância deste projeto é fundamentada em múltiplos aspectos sendo estes:

## Aplicação Interdisciplinar: 
O projeto visa integrar conceitos e práticas das disciplinas de engenharia aeroespacial, automotiva, software, eletrônica e energia, proporcionando aos estudantes uma visão abrangente e interdisciplinar do processo de desenvolvimento de projetos complexos, criado metodologias de trabalho que podem ser usadas na vida profissional do engenheiro.

## Desenvolvimento de Competências Técnicas: 
Participar ativamente na construção de uma mesa giratória com velocidade controlável, capaz de escanear um objeto e posteriormente imprimir em 3D, é um desafio empolgante. No entanto, para garantir que o projeto seja viável, estabelecemos alguns limites: o objeto a ser escaneado e impresso não pode exceder as dimensões de 30x30x30 cm ou pesar mais de 2 kg, incluindo a mesa.

Para alcançar esse objetivo, serão necessários conhecimentos em cálculos estruturais e de resistência dos materiais, eletrônica embarcada e sistemas de controle, análise de dados, priorização e modelagem de requisitos, e desenvolvimento de software embarcado. Além disso, será fundamental desenvolver habilidades de gestão de pessoas para enfrentar os desafios futuros na área da engenharia.

## Desenvolvimento de Soluções Inovadoras: 
O desafio adicional do projeto é coletar informações precisas de um objeto em movimento em uma mesa rotatória. É essencial que esses dados sejam capturados e analisados de forma eficiente para garantir que a impressão em 3D reproduza fielmente o objeto original. A base plana do objeto apresenta uma vantagem, facilitando a análise e o escaneamento.

Para superar esse desafio, será necessário desenvolver um sistema de sensoriamento preciso e confiável, capaz de capturar os dados do objeto em movimento com rapidez e precisão. Além disso, será fundamental implementar algoritmos de processamento de dados eficientes para analisar as informações coletadas e gerar um modelo tridimensional preciso do objeto. Essas etapas são essenciais para garantir que a impressão em 3D reproduza fielmente o objeto original, atendendo aos requisitos do projeto.

## Estímulo à Colaboração:
 O projeto promove ativamente a colaboração entre estudantes de diversas especializações, proporcionando uma experiência similar ao ambiente de trabalho real, no qual equipes multidisciplinares são frequentes e a habilidade de trabalhar em conjunto é essencial.

## Demonstração de Resultados Tangíveis: 
O sucesso do projeto reside em identificar com precisão a velocidade de rotação da mesa giratória, levando em consideração o tempo necessário para que as câmeras realizem a coleta de imagens. Isso é crucial para evitar imagens borradas ou distorcidas que possam resultar em informações imprecisas. Além disso, é fundamental relacionar essas imagens de forma adequada para criar um arquivo tridimensional do objeto, que possa ser utilizado para reproduzi-lo em uma impressora 3D.

Para desenvolver o projeto, é crucial entender o tipo de motor mais adequado para controlar a velocidade de rotação da mesa giratória, levando em consideração o peso do objeto e o tempo necessário para a coleta de imagens. É necessário também considerar como o sistema de motor será alimentado e realizar uma análise energética para compreender sua interação com o problema.

Além disso, é fundamental entender como processar as imagens, incluindo os tipos de componentes, como câmeras, software e hardware, necessários para processar os dados das imagens. É preciso criar um arquivo compatível com a impressora 3D e capaz de produzir uma impressão de qualidade, pois a qualidade do arquivo influencia diretamente na qualidade da impressão final.




## MOTOR DE PASSO

O Motor de Passo é um motor elétrico utilizado em uma infinidade de projetos, como mencionado, sua principal vantagem é a movimentação através de passos ou graus, com isso conseguimos controlar o motor de forma precisa sem o uso de sensores para determinar a posição do motor. Os motores desse tipo são controlados através de sinais digitais enviados para as suas bobinas, possibilitando a rotação fracionada do eixo, sem a necessidade de escovas internas [1].

## Estrutura do Motor de Passo
As características do Motor de Passo, no que diz respeito à velocidade, torque e resolução serão definidas primeiramente pela estrutura do motor, então é importante conhecer os aspectos internos e a função das peças que compõem o motor.

![alt text](../assets/eletronica-energia/image-3.png)

**Figura 1:** Estrutura interna do motor de passo [1].

## Rotor
Uma das partes mais importantes do motor de passo é o rotor, na figura 1, é mostrado  um motor com rotor híbrido, o corpo que representa o rotor híbrido é composto pelos dois rotores e o imã entre eles, utilizado para a polarização do rotor frontal e o traseiro [1].
Existem três configurações possíveis de montagem para o rotor: rotor de imã permanente, rotor de relutância variávele rotor híbrido, o tipo híbrido é o mais comumente utilizado, estas diferenças são apresentadas na tabela 1.

**Tabela 1:** Diferenças entre os rotores
![alt text](../assets/eletronica-energia/image-4.png)

## Estator
O Estator produz o campo magnético que causa a movimentação do rotor. Para análise do estator é necessário tomar nota de alguns pontos como: o número de fases, de par de polos e configuração do fio. A fase ou o par de polos é formado por duplas de bobinas que são energizadas simultaneamente.
A estrutura do estator é formada por polos magnéticos dentados, sendo que cada polo é dotado de uma bobina com o seu par oposto, de forma que os pares são energizados simultaneamente e por consequência são magnetizados com a mesma polaridade, os dois polos formam uma fase. 
O primeiro modelo do exemplo abaixo é do tipo estator bifásico, com fases A e B, enquanto o segundo é do tipo estator trifásico, com fases A, B e C.
![alt text](../assets/eletronica-energia/image-5.png)
**Figura 2:** Modelo de um estator bifásico

![alt text](../assets/eletronica-energia/image-6.png)
**Figura 3:** Estator real

A figura 2, mostra uma representação gráfica da distribuição das bobinas no estator, já a figura 3, mostra uma imagem de um estator real, com seus dentes e bobinas em enrolamento de cobre.
Eixo
O eixo do motor híbrido é construído com dois grupos dentados de rotores, um deles polarizados com polo sul e outro com polo norte.
![alt text](../assets/eletronica-energia/image-7.png)
**Figura 4:** Modelo do eixo do motor [1].
## Tipos de Polos
Existem dois modelos de acordo com os polos, o bipolar e o unipolar, os termos surgiram de conformidade com os drivers que são utilizados para acionamento desses motores. O polar do termo representa “polaridade” e se refere ao driver utilizado para controle desses motores, utilizaremos as expressões “motor unipolar” e “motor bipolar” por convenção social [1].
 
## Unipolar
O modelo utilizado com o driver Unipolar conta com duas bobinas por fase, formando um par de polos, além disso, há o contato em comum, dessa forma os motores desse tipo podem ter 5, 6 ou 8 fios [1].
![alt text](../assets/eletronica-energia/image-8.png)
**Figura 5:** Driver unipolar [1].

Com o fio central é possível controlar a direção da corrente, no entanto apenas metade da bobina pode ser utilizada, isso faz com que o motor seja menos eficiente se comparado ao bipolar. O fio central é conectado ao Vin do circuito, sendo que se o Mosfet 1 estiver ativo, a corrente fluirá de Am para A+, se o Mosfet ativo for o 2, a corrente fluirá de Am para A-.

![alt text](../assets/eletronica-energia/image-9.png)
**Figura 5:** Diagrama circuito unipolar [1].

## Bipolar
No motor do tipo bipolar, cada bobina é composta por dois fios apenas, sem derivações centrais como as do tipo unipolar, de forma que são motores mais fáceis de serem produzidos.

![alt text](../assets/eletronica-energia/image-10.png)

**Figura 7:** Dirver bipolar [1].

Como não há a derivação central, para controle de direção é necessário utilizar uma ponte H, exigindo um circuito de acionamento mais complexo. Para os motores desse tipo, temos que a corrente flui de A- para A+ quando os Mofets 2 e 3 estão ativos, e flui de A+ para A- quando 1 e 4 estão ativos. Apesar de possuir um acionamento mais complexo, os motores do tipo bipolar são mais comuns, pois permitem que o motor atinja maior torque[1].
 
![alt text](../assets/eletronica-energia/image-11.png)

**Figura 8:** Diagrama circuito bipolar [1].

## Funcionamento de um motor de passo:

O motor de passo é um dispositivo eletromecânico composto por bobinas (indutores) e um rotor magnético (ímã permanente ou imantado). As bobinas convertem energia elétrica em campo magnético, alinhando o rotor a esse campo. A excitação correta das bobinas faz o rotor, que gira em torno de seu eixo, mover-se no sentido desejado, convertendo energia magnética em movimento (energia mecânica). O rotor é rotacionado em pequenos incrementos angulares, chamados de "passos" [2].

O funcionamento básico do motor de passo envolve o uso de bobinas alinhadas dois a dois. Quando energizadas, elas atraem o rotor, alinhando-o com o campo magnético gerado, resultando em uma variação angular pequena, chamada de passo. A velocidade e o sentido de movimento são determinados pela forma como cada bobina é ativada, incluindo a ordem e a velocidade entre cada processo de ativação [2]..

As vantagens do motor de passo incluem sua precisão de posicionamento e torque aplicado, além de ter uma resposta excelente na aceleração e desaceleração, devido à sua lógica digital. No entanto, ele pode apresentar baixo desempenho em alta velocidade, requer um certo grau de complexidade para operação e pode sofrer ressonância devido a um controle inadequado [2]..

Complementando com o banco de dados, o motor de passo é frequentemente utilizado em aplicações que exigem precisão de posicionamento, como impressoras 3D, máquinas CNC e robótica industrial. Ele oferece um controle preciso sobre o movimento, o que é essencial em muitas aplicações. Além disso, o motor de passo pode ser facilmente controlado por microcontroladores, o que o torna uma escolha popular em projetos eletrônicos e de automação [2]..

A figura a seguir mostra como um motor de passo pode ser controlado mediante lógica binária
 
![alt text](../assets/eletronica-energia/image-12.png)
**Figura 9:** Motor de passo controlado pelas entradas To até T3 [2].

## PLACA ARDUINO

O Arduino Uno é uma placa microcontrolada baseada no chip ATmega328. Esta placa é muito utilizada no desenvolvimento de projetos embarcados, é hoje em dia é a mais utilizada e documentada da família Arduino.

![alt text](../assets/eletronica-energia/image-13.png)	 

**Figura 10:** Placa Arduino Uno, diagrama de barramento e diagrama esquemático. Fonte(Propria)

A placa conta com um chip ATmega328 que é um microcontrolador único desenvolvido pela Atmel, pertencente à família megaAVR. A arquitetura do Arduino Uno segue o padrão Harvard e possui um núcleo de processador RISC de 8 bits customizado.
![alt text](../assets/eletronica-energia/image-14.png)
**Figura 11:** Diagrama de pinos da placa Arduino Uno [3]


 
## Características principais do Arduino Uno

 - A tensão de operação é 5V
 - A tensão de entrada recomendada varia de 7V a 12V
 - A tensão de entrada varia de 6V a 20V
 - 14 pinos de entrada/saída digital
 - 6 pinos analógicos
 - A corrente DC para cada pino de entrada/saída é de 40 mA
 - A corrente DC para o pino de 3,3 V é 50 mA
 - A memória flash é de 32 KB
 - SRAM é 2KB
 - EEPROM é 1 KB
 - A velocidade do CLK é de 16 MHz

 

## Diagrama de pinos do Arduino Uno

A placa do Arduino Uno conta com uma grande variedade de pinos de alimentação, pinos analógicos, ATmega328, conector ICSP, botão Reset, LED de alimentação, pinos digitais, led de teste, pinos TX/RX, interface USB e fonte de alimentação externa, na figura 11, se apresentam estes pinos.

![alt text](../assets/eletronica-energia/image-15.png)
**Figura 12:** Diagrama de Pinos do microcontrolador ATmega328

A seguir se faz a descrição de cada um deles.

## Descrições principais para utilização do Arduino Uno

## Fonte de Alimentação

Esta placa conta com uma grande vantagem e é poder ligar ela de forma externa com ajuda de um cabo USB ou uma fonte de alimentação externa, além disso, as fontes de alimentação externas incluem principalmente um conversor AC para DC, caso contrário, uma bateria. A fonte deve ser inserida no conector de alimentação da placa Arduino. Suas faxas de tensão estão entre 7 e 12 Volts,  conta com um pino GND e conector POWER.[3]

 

## Entradas e saídas digitais

O Arduino Uno possui 14 pinos que podem ser usados como entrada ou saída a depender da necessidade do programador. Com a ajuda de funções como pinMode(), digitalWrite() e Digital Read() é possível definir como os pinos serão utilizados [3].

 

## Entradas analógicas

A placa Arduino UNO conta com 6 canais de conversor analógico para digital, nomeadas de A0 a A5. Sendo que a resolução do conversor analógico digital é de 10Bits. Isso significa que este irá mapear tensões entre 0 e a tensão operacional (5V ou 3.3V) para valores inteiros entre 0 e 1023. No Arduino UNO, isso permite uma resolução entre leituras de: 5 volts / 1024 unidades, ou .0049 volts (4.9 mV) por unidade. Essas entradas são nomeadas de A0 a A5. A função analogRead() lê o valor de um pino analógico especificado [3].

 

## Pino (TX) e Pino (RX) (Serial):

Os pinos 0 e 1 são usados para transmitir e receber dados seriais TTL, e estes são conectados aos pinos equivalentes do chip ATmega8U2 USB para TTL Serial [3].

 

## Pinos externos de interrupção:

Os pinos 2 e 3 do Arduino Uno podem desempenhar a função de entrada de sinal para interrupção externa tais funções são nomeadas de INT0 e INT1, respectivamente [3].

 

## Pinos 3, 5, 6, 9, 10 e 11 (PWM):

O Arduino Uno possui 6 pinos para saída PWM, são estes os pinos 3,5,6,9,10 e 11. Para auxiliar na manipulação desses pinos a plataforma possui uma função que auxilia na escrita de valores chamada de “duty cycle” facilitando a utilização do PWM do Arduino Uno, o qual pode ser acoplado com módulos externos [3].

 

## Pinos SPI (Pino-10 (SS), Pino-11 (MOSI), Pino-12 (MISO), Pino-13 (SCK):

SPI (Serial Peripheral Interface) é um protocolo de comunicação serial, a SPI possui uma conexão full duplex, o que significa que os dados são enviados e recebidos simultaneamente. O SPI pode ser utilizado para a comunicação entre dois arduinos [3].

 

## LED Interno Pino 13

A placa do Arduino Uno possui um Led interno conectado ao pino 13(pino digital). Como pino de valor ALTO, o diodo emissor de luz é ativado, sempre que o pino estiver em nível BAIXO [3].

 

## Pino-4 (SDA) e Pino-5 (SCL) (I2C):

Permite comunicação TWI (Two Wire Interface) com a ajuda da biblioteca Wire [3].

 

## AREF (Tensão de Referência):

AREF significa Referência Analógica. Ele permite alimentar o Arduino com uma tensão de referência de uma fonte de alimentação externa para configurar a tensão de referência usada para entrada analógica (ou seja, o valor usado como o topo da faixa de entrada) [3].

## Pino de Reset:

Este pino é usado para resetar (RST) o microcontrolador [3].

 
## Memória

A memória do microcontrolador Atmega328 do Arduino Uno inclui memória flash de 32 KB para armazenamento de código, SRAM-2 KB e EEPROM-1 KB [3].

 

## Comunicação

O Arduino Uno ATmega328 oferece comunicação serial UART TTL e é acessível em pinos digitais como TX (1) e RX (0). O software de um Arduino possui um monitor serial que permite dados fáceis. Existem dois LEDs na placa, como RX e TX, que piscarão sempre que os dados estiverem sendo transmitidos através do USB.

 

A biblioteca SoftwareSerial permite a comunicação serial nos pinos digitais do Arduino Uno e o ATmega328P suporta TWI (I2C), bem como comunicação SPI. O software Arduino contém uma biblioteca cabeada para simplificar a utilização do barramento I2C [3].

 

## Proteção de alta tensão do USB

A placa Arduino Uno possui um fusível que protege a porta USB do PC de sobretensão. Embora a maioria dos PCs tenha sua própria proteção interna, o fusível oferece uma proteção adicional de segurança [3].

 

## Características físicas

As características físicas de uma placa Arduino incluem principalmente comprimento e largura. O comprimento e a largura da placa de circuito impresso do Arduino Uno são 2,7 X 2,1 polegadas, mas o conector de alimentação e o conector USB se estenderão além dessa medida. A placa pode ser fixada na superfície, caso contrário, com os orifícios dos parafusos [3].


## Ponte H, Driver L298N:

Este componente facilita o projeto do controle PWM, por nele encontra-se toda a configuração de portas lógicas, transistores e capacitores para realizar a modulação, ele tem as seguintes especificações segundo o fabricante.

## Especificações:

- Tensão de Operação: 4.5 V a 46 V
- Controle de 2 motores DC ou 1 motor de passo
- Corrente de Operação máxima: 2 A por canal ou 4 A total
- Tensão lógica: 4.5 V a 7 V
- Corrente lógica: 0 a 36 mA
- Limites de Temperatura: -20°C a +135°C
- Potência Máxima: 25 W
- Dimensões: 43 x 43 x 27 mm


As pontes H  utilizam quatro transistores que, ao receber um sinal vindo do microcontrolador, permitem a passagem de corrente para os terminais do motor, fazendo com que ele rotacione no sentido desejado, esta ponde encontra-se no driver L298N utiliza duas pontes H para controlar separadamente dois motores. Porém, além de controlar o sentido de rotação do motor, o driver também é capaz de controlar a velocidade do motor. Utiliza-se um sinal PWM para regular o nível de rotação do eixo. 

A modulação por largura de pulso (PWM) é uma técnica fundamental que envolve a variação da largura dos pulsos em um sinal elétrico para transmitir informações. Em vez de manter um sinal em níveis constantes, o PWM altera a largura dos pulsos, controlando o tempo em que a chave fica ligada e desligada. Isso permite administrar a quantidade média de energia que chega à carga e, consequentemente, a potência elétrica [4].

Essa técnica é amplamente utilizada em diversos equipamentos eletrônicos de potência, como drivers de LED, inversores de frequência e controle de velocidade de motores. No cotidiano, o PWM é encontrado em carregadores, sistemas fotovoltaicos, servo-motores e carros elétricos, entre outros [7].

O ciclo de trabalho, ou Duty Cycle mostrado na figura, é um parâmetro crucial para controlar um sinal PWM. Ele representa a relação entre a largura do pulso e o período, informando o tempo em que o sinal está em nível alto (ligado) e o tempo em que está em nível baixo (desligado). O Duty Cycle é expresso em porcentagem e calculado pela fórmula D = (PW / T) x 100%, onde PW é a largura do pulso e T é o período [7]. Deste modo, o sinal 255 da placa é convertido para um sinal PWM de 100%, e o sinal 0 da placa é convertido para um sinal PWM de 0%. Portanto um sinal de 127 da placa será convertido para um sinal PWM de 50%. Consequentemente, para um motor, o sinal 0 seria o motor parado, já o sinal 255 seria a sua rotação máxima. Abaixo é possível ver um exemplo com o sinal PWM sendo aplicado em um LED [5].

![alt text](../assets/eletronica-energia/image-16.png)
**Figura 13:** Representação do comportamento do controle PWM

Uma das principais vantagens do PWM é a manutenção do sinal digital em todo o percurso, o que minimiza os efeitos de ruído. Além disso, o PWM oferece maior imunidade ao ruído em comparação ao controle analógico, o que torna essa técnica ideal para comunicações. Em sistemas de freios controlados por modulação, por exemplo, o PWM é utilizado para controlar a pressão exercida pelo freio de acordo com a quantidade de tensão ou corrente aplicada [4].

![alt text](../assets/eletronica-energia/image-17.png)
**Figura 14:** Funcionamento do PWM num led.
Fonte [5]

## Funcionamento do Driver L298N

O módulo L298N utiliza as portas In1, In2 e EnA para controlar o motor "A" (lado esquerdo do diagrama de blocos da imagem da figura 11). Os pinos In1 e In2 são responsáveis pelo direcionamento do sentido do motor, e o pino EnA é responsável pela regulação de velocidade do motor "A", portanto o pino de saída da BlackBoard para o pino EnA do módulo deverá permitir um sinal PWM. Da mesma maneira que o motor "A", o motor "B" possui dois pinos de direcionamento de sentido, porém ao invés de serem os pinos In1 e In2, são os pinos In3 e In4. O pino que determina a velocidade do motor "B" é o EnB, que também deve permitir um sinal PWM vindo da BlackBoard. É possível observar o diagrama de blocos do funcionamento do chip L298N figura 11.
 
 ![alt text](../assets/eletronica-energia/image-14.png)
**Figura 15:** Diagrama de blocos do L298M
Fonte [7]

Rampa de Aceleração e Desaceleração
É utilizada uma rampa de aceleração e desaceleração para fazer com que o motor gire. A rampa de aceleração irá aumentar a velocidade do motor gradativamente até que ele atinja a sua velocidade máxima. Já a rampa de desaceleração fará o oposto com o motor, desacelerando gradativamente, na mesma proporção acelerada. Essa rampa de aceleração é utilizada para evitar que o motor atinja um pico de corrente ao ser partido [5]. 
 
 ![alt text](../assets/eletronica-energia/image-15.png)
**Figura 16:** Rampa de aceleração de desaceleração do drive L298N
Fonte [5]

Assim conhecendo todos os componentes, foi montada uma simulação utilizando programa Proteus, a qual é motrada na figura 13. A figura 14 representa o mesmo circuito montado no software Fritzing, com a finalidade de mostrar como ele seria montado de forma real na protoboard, a figura 15  mostra o diagrama de barramentos, e a figura 16 o diamgrama esquemático do circuito.

## Descrição matemática do MOTOR

Um motor pode ser modelado utilizando um Resistor, um indutor e uma força contra eletromotriz que relaciona o fluxo magnético gerado pelo motor em função do fluxo magnético e do número de espiras que ele tem, sendo assim esta força é modelada pela relação de Faraday como se mostra na equação 1:

![alt text](../assets/eletronica-energia/image-24.png)
## miguel

A equação que representa a tensão pode ser modelada aplicando a LKT, representada como mostra a equação 2 e a figura 17:

![alt text](../assets/eletronica-energia/image-25.png)

![alt text](../assets/eletronica-energia/image.png)
**Figura 17:** Modelo Elétrico do motor DC

O motor pode ser separado em variáveis elétricas e mecânicas, conforme mostra a figura 4, onde a parte ressaltada na cor preto, indica a parte elétrica e a ressaltada na cor vermelho a parte mecânica como.

![alt text](../assets/eletronica-energia/image-1.png)

**Figura 18:** Modelo elétrico e mecânico do motor DC

![alt text](../assets/eletronica-energia/image-26.png)

O campo incidente sobre o motor é chamado campo fixo, esse campo fixo pode ser gerado por uma bobina ou imã permanente, supondo que a corrente elétrica de campo constante, descartando efeitos secundários, em uma máquina rotativa a variação do fluxo magnético sobre a bobina é proporcionar a velocidade angular como mostra a equação 3.

![alt text](../assets/eletronica-energia/image-42.png)

**Figura 19:** Representação do campo magnético no motor

![alt text](../assets/eletronica-energia/image-27.png)

Assim a força contra eletromotriz é proporcional ao fluxo, desta forma pode ser representada como mostra a equação 4:

![alt text](../assets/eletronica-energia/image-28.png)

Como a força exercida nos condutores é proporcional à corrente elétrica que passa pelo condutor, o torque do motor é proporcional à corrente, e se iguala quando se utiliza uma constante de torque \( Kt \), como mostra a equação 5.

![alt text](../assets/eletronica-energia/image-29.png)

Assim a potência é produto do torque pela velocidade angular desenvolvida pelo motor, desta forma:

![alt text](../assets/eletronica-energia/image-30.png)

Outro parâmetro considerado é o torque inercial, o qual tem como trabalho suprimir todas as perdas e ser suficiente para acelerar o motor até um ponto de inércia, ele pode ser representado como a equação 7:

![alt text](../assets/eletronica-energia/image-31.png)

![alt text](../assets/eletronica-energia/image-32.png)

O torque total de atrito do motor ou de arrasto, depende da velocidade angular do motor, ele é dependente do coeficiente de arrasto ou atrito viscoso do motor, assim o torque total do motor é:

![alt text](../assets/eletronica-energia/image-33.png)

Substituindo o torque total, encontra-se a relação de corrente como mostra a equação 9:

![alt text](../assets/eletronica-energia/image-34.png)

Substituído a corrente na equação geral do motor, encontramos a representação da velocidade angular em função da velocidade de entrada do motor, como mostra equação 10:

![alt text](../assets/eletronica-energia/image-35.png)

Realizando procedimentos matemáticos, e derivando o termo do indutor e reagrupando termos é obtida a equação diferencial não homogênea mostrada na equação 11:

![alt text](../assets/eletronica-energia/image-36.png)

A velocidade máxima pode ser calculada como:

![alt text](../assets/eletronica-energia/image-37.png)

Aplicando a transformada de Laplace para a EDO com condições iniciais nulas, encontra-se a função de transferência geral descrita na equação:

![alt text](../assets/eletronica-energia/image-38.png)

## Cálculo dos Parâmetros do Motor
Para calcular os parâmetros do motor, é necessário conhecer as características dele publicadas pelo fabricante, considerando que os motores de passo tem o código NEMA 17 4.2Kgf 1.7A (Stepper Motor 17HS4401).

As especificações são as seguintes:
## ESPECIFICAÇÕES DO MOTOR DE PASSO

- Ângulo do passo: 1.8°
- Tensão de Retenção: 3V
- Tensão nominal: 4,8V
- Resistência: ~1.8 Ohms
- Inércia do Rotor: 38g cm²
- Corrente de Retenção: 1.7A
- Rosca frontal: M3
- Enrolamento: Espiras bifilares
- Temperatura máxima de operação: 80°C
- Temperatura ambiente: -10°C a 50°C
- Classe de isolamento: B
- Torque: 4,2Kgf.cm
- Indutância por Fase: 2,3mH
- Quantidade de fios: 4
- Comprimento do cabo: 100cm
- Comprimento do eixo exposto: 20mm
- Diâmetro do eixo: 5mm
- Dimensões do motor (CxLxA): 42x42x39mm (ignorando o eixo)
- Peso do motor: 280g

Os cálculos feitos são apresentado na seguinte tabela 2:

**Tabela 2:** Cálculos do motor de passo.
![alt text](../assets/eletronica-energia/image-39.png)

Substituindo na função de transferência mostrada na equação 12, é encontrada a representação do motor DC:
![alt text](../assets/eletronica-energia/image-40.png)




A equação diferencial é representada como:
![alt text](../assets/eletronica-energia/image-41.png)

Fazendo uma representação da função de transferência utilizando um degrau unitário, foi encontrado o comportamento mostrado na figura 6.
![alt text](../assets/eletronica-energia/motor1.png)
**Figura 20:** Função de transferência do motor de Passo.

É observado que o comporamento matemático do motor passo tem um comportamento de primeira ordem, más, na equação 12, foi mostrado que este era de segunda ordem, o que indica que o efieto de segunda ordem é pouco relevante para este sistema, por esse motivo foi feita uma aproximação para um modelo de primeira ordem, assim, foi feito um procedimento matemático para encontrar essa aproximação considerando que o termo de segunda ordem está em relação ao indutor, e sua contribuição é pequena, este parâmetro foi aproximado a zero, assim a EDO da equação 11 fica como mostra a equação 13


![alt text](../assets/eletronica-energia/image-43.png)

![alt text](../assets/eletronica-energia/image-44.png)

Fazendo a representação da equação de transferência proposta na equação 15 e comparando com a função de transferência mostrada na equação 14, é verificado, que efetivamente o sistema pode ser representado como um sistema de primeira ordem, pois as duas respostas são idênticas.

![alt text](../assets/eletronica-energia/motor2.png)
**Figura 21:** Compração do sistema de primeira e segunda ordem.



## Modelo do circuito

O circuito precisa de um módulo que permita trabalhar com duas tensões, uma de 12V para alimentar a Ponte H, e um de 5V para alimentar a placa de árduino, para resolver esta situação foi trabalhado com um fonte de 12V e um módulo regular C/LM2596, Oo Módulo Regulador de Tensão LM2596 trabalha como um conversor DC DC no modo Step Down, sendo capaz de reduzir uma carga de até 3A com ótima eficiência. A tensão de saída pode ser ajustada entre 1,5 a 35v, tendo como entrada 3,2 a 40v. Possui uma velocidade de comutação de 150KHz e pode ser aplicado em circuitos onde a saída de um sensor é superior a 5v, tensão de entrada máxima em um Arduino ou PIC [8].

![alt text](../assets/eletronica-energia/image-18.png)

**Figura 22:** Módulo regular C/LM2596

Já a figura 21, apresenta o regulador especificando como identificar as conexões tanto de entrada como de saída.

![alt text](../assets/eletronica-energia/image-20.png)
**Figura 23:** Especificação dos componentes do módulo regulador C/LM2596

Este módulo tem as seguintes carácterísticas:
![alt text](../assets/eletronica-energia/image-19.png)

Já definidos os  módulos e os motores, foi proposto o seguinte modelo circuital apresentado nas figuras 24 e 25, que mostram com são feitas as conexões:

![alt text](../assets/eletronica-energia/image-45.png)
**Figura 24:** Modelo do circuito a ser implementado.


![alt text](../assets/eletronica-energia/image-21.png)
**Figura 25:** Representação da simulação do circuito com dois motores

## Diagrama Esquemático do circuito Eletrônico
Após ter finalizado a simulação foi criado utilizando o software Fritzing o diagrama esquemático que representa o circuito, o qual é mostrado na figura 26.

![alt text](../assets/eletronica-energia/image-22.png)
**Figura 26:** Diagrama esquemático do circuito elétrico

## Diagrama detalahado de Barramentos do Circuito do circuito eletrônico
Seguidamente foi gerado o diagrama completo de barramentos que especifica como devem ser as conexões na placa que será implementado o circuito, este é mostrado na figura 27

![alt text](../assets/eletronica-energia/image-23.png)
**Figura 27:** Diagrama completo de Barramentos do circuito.


## Diagrama com detalhes dos protocolos de comunicaçãos entre os elementos.
Até o momento no desenvolvimento da pesquisa, no circuito simulado e testado não temos protocolos de comunicação, pois, os dados são uniderecionados e o controle está relacionado com tensão. Foi identificado que estes protocolos de comunicação estão mais relacionados com a etapa de software que trabalhará com a coleta de dados e o processamento dos mesmos.


## REFERÊNCIAS BIBLIOGRÁFICAS:

[1]curto circuito, introdução ao motor de passo, https://curtocircuito.com.br/blog/motor-de-passo/introducao-ao-motor-de-passo,acesso 19:04 hora: 13:17

[2] fpg Paratodos, Controle de motor de passo,http://fpgaparatodos.com.br/2012/03/30/controle-de-um-motor-de-passo/ acesso 19/04/2024 hora 13:16

[3] STA, Sistema de Tecnología aplicada, Ronteck,CARACTERÍSTICAS PRINCIPAIS DO ARDUINO UNO,https://www.sta-eletronica.com.br/artigos/arduinos/caracteristicas-principais-do-arduino-uno, Acesso, 12/04/2024 hora 16:00

[4] O que é PWM e Para que Serve?,  Cristiano Bertulucci Silveira, publicado: novembro 26th, 2016, citisystems, acesso 16/04, hora 13:28, https://www.citisystems.com.br/pwm/

[5] Robocore, PonteH,https://www.robocore.net/tutoriais/motor-dc-arduino-ponte-h-l298n, Acesso 16/04/2024, hora 13:33.

[6] Datasheet - L298 - Dual full-bridge driver, https://www.st.com/resource/en/datasheet/l298.pdf

[7] Smart kits blog,https://blog.smartkits.com.br/pwm-como-usar/#:~:text=O%20PWM%20opera%20controlando%20o,%2C%20consequentemente%2C%20a%20pot%C3%AAncia%20el%C3%A9trica, Acesso, 16/04/2024, hora 13:26 

[8] Casa da Robótica, egulador de Tensão Step Down - Buck Conversor DC DC LM2596 3A, https://www.casadarobotica.com/fonte-e-conversores/conversores-dc-dc/step-down/regulador-de-tensao-step-down-buck-conversor-dc-dc-lm2596-3a, acesso 26/04/2024, hora: 20:25
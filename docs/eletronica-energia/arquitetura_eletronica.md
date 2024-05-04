## Arquitetura do Subsistema de Eletrônica

<p style="text-align:justify;"> Neste capítulo do projeto, faz-se uma descrição teórica dos componentes que serão inicialmente utilizados neste trabalho, ressaltando que alguns deles podem ser modificados em função de ajustes que sejam necessários futuramente. </p>

<p style="text-align:justify;"> Inicia-se descrevendo o motor de passo e suas características e estrutura interna, especificando cada um de seus componentes. Posteriormente, inicia-se a descrição dos componentes eletrônicos, começando pela placa Arduino Uno, que será fundamental para o desenvolvimento do projeto. Com ela, serão realizados os diferentes controles, sendo um Arduino para manipular os dados de escaneamento que devem ser processados, e outro Arduino para controlar dois motores de passo: o primeiro para controlar o giro da mesa e o segundo para controlar a altura da câmera que fará a coleta de dados. São descritas todas as características que este microcontrolador possui e que podem ser utilizadas para desenvolver este trabalho. </p>

<p style="text-align:justify;"> Em seguida, é feita a descrição da ponte H, um componente com o código L298N, apresentando suas características. A funcionalidade deste componente é facilitar a comunicação dos motores com o Arduino e, assim, possibilitar o controle proposto. </p>

<p style="text-align:justify;"> Dado que o sistema possui dois motores de passo que necessitam de uma alimentação de 12V e circuitos integrados que requerem uma tensão de 5V, torna-se necessário o uso de uma bateria de 12V para alimentar os motores e o uso de mais um dispositivo regulador, como o LM2596, que permite obter a tensão necessária para a alimentação da parte eletrônica. </p>

<p style="text-align:justify;"> Posteriormente, após a identificação dos componentes que serão utilizados, é feita a descrição matemática do motor de passo, gerando uma função de transferência para conhecer o comportamento da velocidade de giro em função do tempo. Esta caracterização do motor foi feita utilizando as características técnicas fornecidas pelo fabricante. </p>

<p style="text-align:justify;"> O capítulo é finalizado mostrando imagens de simulação dos circuitos utilizando Proteus e Fritzing, e a geração dos diagramas de blocos do circuito e o diagrama de barramento para a parte dos motores.</p>

## Versionamento

| Versão | Data       | Modificação             | Autor       |
| ------ | ---------- | ----------------------- | ----------- |
| 0.1    | 03/05/2024 | Criação do documento    | Carolina Oliveira, Miguel Munoz |
| 0.2    | 03/05/2024 | Adição de versionamento | Ciro Costa  |
| 0.3    | 04/05/2024 | Ajustes de formatação | Ana Carolina |

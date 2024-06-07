# Arquitetura do Subsistema de Eletrônica

<p style="text-align:justify;">
O principal objetivo da execução do projeto do subsistema eletrônico é de garantir o controle preciso e eficiente do sistema, permitindo o funcionamento adequado do scanner e da mesa rotatória. Para isso, é necessário selecionar e integrar os componentes eletrônicos de forma a atender aos requisitos funcionais e não funcionais estabelecidos.
</p>

<p style="text-align:justify;">
A arquitetura do subsistema envolve motores de passo, microcontroladores Arduino Uno, a ponte H (L298N) e um regulador de tensão LM2596. Os motores de passo controlam a rotação da mesa e a altura da câmera, enquanto os microcontroladores Arduino Uno manipulam os dados de escaneamento e controlam os motores. A ponte H facilita a comunicação entre os motores e os Arduinos, permitindo o controle bidirecional necessário.
</p>

<p style="text-align:justify;">
A alimentação do sistema é fornecida por uma bateria de 12V, com o regulador de tensão LM2596 ajustando a tensão para 5V, conforme necessário para os componentes eletrônicos. Essa configuração assegura que todos os elementos do sistema recebam a energia adequada para um funcionamento estável e eficiente.
</p>

<p style="text-align:justify;">
Ao longo do desenvolvimento, serão realizadas simulações dos circuitos utilizando softwares como Proteus e Fritzing. Essas simulações, juntamente com diagramas de blocos do circuito e diagramas de barramento, proporcionarão uma visão abrangente e detalhada da arquitetura do subsistema eletrônico, facilitando a compreensão e verificação do projeto. 
</p>

## Versionamento

| Versão | Data       | Modificação             | Autor       |
| ------ | ---------- | ----------------------- | ----------- |
| 0.1    | 03/05/2024 | Criação do documento    | Carolina Oliveira, Miguel Munoz |
| 0.2    | 03/05/2024 | Adição de versionamento | Ciro Costa  |
| 0.3    | 04/05/2024 | Ajustes de formatação | Ana Carolina |
| 0.4    | 04/05/2024 | Atualização da formatação | Carolina |
| 1.0    | 07/06/2024 | Adequação da Arquitetura conforme feedback do PC 1 | Carolina |

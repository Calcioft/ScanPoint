
# Arquitetura do Subsistema de Software

A arquitetura de software está dividida nos seguintes componentes:

- Aplicação: Desenvolvida em Electron, cuida de toda a interação com usuário e sinais para comunicação com o embarcado
- Embarcado: Usando uma Arduino, ela faz a comunicação com o sensor;
- Sensor Infravermelho: Irá ler todo o item a ser escaneado;
- Motor de rotação: Irá girar a mesa onde o item está posicionado, possibilitanto os vários ângulos para reconstrução 3D;
- Motor de regulação de altura: Irá possibilitar a regulação da altura do sensor infravermelho, assim possibitando uma melhor leitura de itens de diversos tamanhos.

A relação entre os componentes está elencada no diagrama abaixo:

## Diagrama de arquitetura de software 

![](/assets/software/Diagrama-arquitetura-software.png)


# Arquitetura de Software

Esta sessão elenca todos os itens de arquitetura de software, como os componentes utilizados e sua comunicação e as tecnologias utilizadas.

## Componentes 

A arquitetura de software está dividida nos seguintes componentes:

- Aplicação: Desenvolvida em Electron, cuida de toda a interação com usuário e sinais para comunicação com o embarcado. Ela possui um front-end com opções iterativas para o usuário controlar o sistema;
- Script de conversão: Vai converter o arquivo de texto com as informações espaciais do objeto e transformar em .stl(formato para impressão 3D)
- Embarcado: Usando uma Arduino, ela faz a comunicação com os componentes do sistema e retorna o arquivo de texto com os dados espaciais do objeto;
- Sensor Infravermelho: Irá fazer a leitura de distâncias, mapeando o objeto;
- Motor de rotação: Irá girar a mesa onde o item está posicionado, possibilitanto a leitura do objeto em 360 graus;
- Motor de regulação de altura: Irá possibilitar a regulação da altura do sensor infravermelho, assim passando por todo o comprimento do objeto;

A relação entre os componentes está elencada no diagrama abaixo:

## Diagrama de arquitetura de software 

![](/docs/assets/software/diagrama-arquitetura.png)

## Tecnologias

AS tecnologias de software utilizadas nesse projeto foram:

- Electron: É um framework open-source para criar aplicações Desktop usando tecnologias web para Windows, mac e Linux, com base no Chromium e Node.js;

- Arduino: É uma plataforma open-source com hardware e software com fácil aprendizagem. As placas Arduino tem a capassidade de registrar entradas diferentes, como botões, sinais de sensores, etc. Para programar as placas, existe o Arduino IDE (que é multiplataforma), com sua própria linguagem de programação.

## Referências
- [What is Electron? Acesso em 28 de abril de 2024.](https://www.electronjs.org/docs/latest/)

- [What is Arduino? Acesso em 28 de abril de 2024.](https://docs.arduino.cc/learn/starting-guide/whats-arduino/?_gl=1*23ysxj*_ga*MTE4MTM4NjIyMS4xNzE0MzI5NTA3*_ga_NEXN8H46L5*MTcxNDMyOTUwNi4xLjEuMTcxNDMyOTU0MS4wLjAuMTI1MzcwNzA4Mw..*_fplc*cTIzWiUyRjhGOVMlMkZVbUlwOXY4U2ptYnJXUEJXUER4ODFoZUg3c1g3QkNVT3djVkpoRTF5MEE0dVBIYlVWRmI3RGlZVHJXNHZlMm5KUmhhcVJHSTc5RW5CSWtCVDFSRGd1SjVhR08wNXlWSW1EZGVKTHZORm5mTzJVajk3QWFtdyUzRCUzRA..)





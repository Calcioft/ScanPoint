# Arquitetura do Subsistema de Software

## Arquitetura de Software

A arquitetura do software está definida no diagrama abaixo, sendo dividido no aplicativo, no conversor, no embarcado, sensor infravermelho e dois motores:

![](/assets/software/diagrama-arquitetura.png)

Para atingir os objetivo será utilizado duas tecnologias: Electron, para o aplicativo e Arduino, para o embarcado.

Mais detalhes na pagina de [Arquitetura de Software](/software/arquitetura)

## Interface

## Arduino

O Arduino é responsável por receber dados provenientes dos sensores, realizando o processamento necessário e transmitindo essas informações para a aplicação Electron. Além disso, assume o controle dos motores, gerenciando seu funcionamento e movimentação de acordo com as instruções fornecidas pela aplicação.

No âmbito operacional, o Arduino opera como uma unidade mestra, coordenando e controlando o fluxo de dados entre os diferentes componentes do sistema.git 

## Software de Processamento PointCloud

Após a leitura de todos os pontos de distância feito pelos sensores ligados ao arduíno, o arquivo .txt gerado deve ser passado por um script de conversão desenvolvido em Python, usando a biblioteca NumPy.

No geral ele irá ler todos os valores de distância do arquivo txt e irá processar os dados, aplicando a distância do sensor ao ponto de leitura, transformar em uma matrix de rotação e depois em pontos catesianos. Em seguida elimina todos os pontos fora de alcance do sensor e passa todos os valores para ser convertido em STL.


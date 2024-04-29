# Arquitetura do Subsistema de Software

## Arquitetura de Software

A arquitetura do software está definida no diagrama abaixo, sendo dividido no aplicativo, no conversor, no embarcado, sensor infravermelho e dois motores:

![](/assets/software/diagrama-arquitetura.png)

Para atingir os objetivo será utilizado duas tecnologias: Electron, para o aplicativo e Arduino, para o embarcado.

Mais detalhes na pagina de [Arquitetura de Software](/software/arquitetura)

## Interface

## Arduino

## Software de Processamento PointCloud

Após a leitura de todos os pontos de distância feito pelos sensores ligados ao arduíno, o arquivo .txt gerado deve ser passado por um script de conversão desenvolvido em Python, usando a biblioteca NumPy.

No geral ele irá ler todos os valores de distância do arquivo txt e irá processar os dados, aplicando a distância do sensor ao ponto de leitura, transformar em uma matrix de rotação e depois em pontos catesianos. Em seguida elimina todos os pontos fora de alcance do sensor e passa todos os valores para ser convertido em STL.


# Termo de abertura de projeto

## Dados do projeto 

- **Nome do Projeto**: ScanPoint
- **Data de abertura**: 29/03/2024
- **Código**: 1-A
- **Patrocinador**: Universidade de Brasília (UnB) 
- **Gerente/Coordenadora Geral**: Carla Rocha 

## Descrição do projeto 

<p style="text-align: justify;"> O presente projeto, intitulado ScanPoint, encontrasse inserido no âmbito da disciplina de Projeto Integrador 2 e surge como uma resposta à necessidade crescente de simplificar e otimizar o processo de digitalização e reprodução tridimensional de objetos físicos. O projeto é formado por uma mesa escaner e um aplicativo desktop. A mesa escaner é composta por um Arduino e sensores infravermelho que realizam a captura pontos de distância dos objetos. O aplicativo desktop é responsável pela interação com o usuário e por processar os pontos enviados pela mesa, de modo que gere um arquivo em stl que permite o objeto ser reproduzido por uma impressora 3D. </p>

## Justificativa do projeto 
<p style="text-align: justify;"> A tecnologia de impressão 3D tem ganhado cada vez mais espaço no mercado, tanto no âmbito industrial quanto no pessoal. Para realizar a impressão de um objeto em 3D é indispensável um arquivo stl, no entanto, o conhecimento necessário para gerar este arquivo não é comum. Visando simplificar e agilizar o processo de reprodução de objetos tridimensionais surgiu o presente projeto.</p>

## Objetivos 

<p style="text-align: justify;"> O projeto ScanPoint tem como objetivo principal desenvolver um sistema que simplifique o processo de escaneamento e reprodução tridimensional de objetos físicos. A proposta visa fornecer uma solução completa, acessível e intuitiva, permitindo aos usuários a digitalização de objetos para a geração de modelos 3D e a subsequente criação de arquivos prontos para impressão tridimensional.</p>

## Gerente de projeto - responsabilidades e autoridades

<p style="text-align: justify;"> Carla Rocha Cangussú desempenha o papel de Coordenadora Geral no projeto, assumindo uma série de responsabilidades essenciais. Isso inclui liderar a equipe, assegurar o cumprimento integral do escopo, prazos e orçamento. Além disso, ela coordena todas as atividades do projeto, identificando e mitigando riscos, e mantendo uma comunicação eficiente entre todas as partes envolvidas. Possuindo autoridade para tomar decisões que impactam diretamente o progresso e o sucesso do projeto, Carla também atua como representante da equipe diante das partes interessadas, garantindo uma colaboração fluida e produtiva.</p>

## Partes Interessadas

###  Professores Orientadores:
<p style="text-align: justify;">Os professores orientadores desempenham um papel crucial na supervisão e orientação deste projeto. Sua contribuição envolve o acompanhamento detalhado do progresso, fornecimento de orientações técnicas, insights estratégicos e avaliação crítica. Sua vasta expertise é essencial para garantir a qualidade e eficácia do projeto de escamento de objetos 3D, fornecendo orientações valiosas à equipe.</p>

### Graduandos de Engenharia:
<p style="text-align: justify;">Os graduandos de engenharia formam a equipe executora deste projeto. Eles têm a responsabilidade de implementar as soluções propostas, desenvolver o sistema, integrar os componentes e garantir sua funcionalidade adequada. Sua dedicação, habilidades técnicas e colaboração são fundamentais para alcançar com sucesso os objetivos e entregas deste projeto.</p>

### Usuários Finais:
<p style="text-align: justify;">Os usuários finais deste projeto são pessoas que desejam replicar objetos em 3D, que se beneficiarão diretamente do escaneamento e da geração dos arquivos prontos para impressão tridimensional. Sua experiência e feedback desempenham um papel crucial na validação e aprimoramento contínuo do sistema. Uma interação próxima e contínua com esses usuários é essencial para garantir que o sistema atenda plenamente às suas necessidades e otimize sua experiência de interação com o sistema.</p>

##  Descrição do produto do projeto

### Subproduto de Software
<p style="text-align: justify;">O subproduto de software é um aplicativo desktop e um sistema embarcado. O sistema embarcado tem como atribuição a coleta de pontos de distância do objeto. O aplicativo é responsável pela interação com o usuário e por processar os pontos coletados, de modo que gere um arquivo em stl que permite o objeto ser reproduzido por uma impressora 3D. </p>

### Subproduto de Eletrônica
<p style="text-align: justify;">Este subproduto envolve a seleção e integração dos motores, do arduino, do Módulo regular C/LM2596 e o driver L298N.</p>

### Subproduto de Estrutura
<p style="text-align: justify;">O subproduto de Estrutura  é composto por uma estrutura de alumínio que delimita o tamanho do objetos e facilita seu transporte ,  uma caixa para abrigar os componentes eletrônicos e fontes de energia, uma estrutura  para elevar o sensor e um prato giratório.</p>

### Subproduto Energia
<p style="text-align: justify;">O subproduto de energia desempenha um papel vital ao alimentar os demais subsistemas, assegurando eficiência energética e operacional. É neste subproduto que é dimensinado o consumo energético, selecionados os componentes de baixo consumo e implementadas as estratégias de gerenciamento de energia em conformidade com as normas de segurança pertinentes.</p>

## Orçamento inicial 

<p style="text-align: justify;">Durante a fase inicial de planejamento orçamentário, o grupo conduziu uma pesquisa para identificar todos os elementos essenciais para a execução do projeto. É relevante destacar que determinados itens, como o Fuso 8mm x 450mm, a castanha 8mm, as extrusões de alumínio (20mmx20mmx500mm e 20mmx40mmx500mm), Arduino UNO, Chave botão, Resistor de filme de carbono 1R - 1/4W, motor DC com engrenagem de redução 6, Módulo Ponte Duplo H Hg7881 para motor DC, Passo, Transistor BJT, diodo (Schottky), Protoboard de 400 pontos, Motor de Passo e uma bateria, já estão disponíveis, o que elimina a necessidade de aquisição e contribui consideravelmente para a redução dos custos totais do projeto. O orçamento inicial, levando em conta apenas os equipamentos e serviços que precisam ser adquiridos, foi estimado em aproximadamente R$ 494,01. Ao dividir esse valor entre os membros do grupo, resultou em uma quantia aproximada de R$ 33,00 para cada integrante.</p>

Para mais detalhes acesse o documento de [Estimativa de Custos](docs/geral/estimativa-custos.md).

## Restrições e riscos

Os riscos podem ser encontrados no documento de [Levantamento de riscos](docs/geral/FMEA.md).

## Cronograma dos marcos do projeto
<p style="text-align: justify;">O projeto segue um cronograma definido com três marcos principais, conforme apresentado na tabela abaixo. O primeiro marco está agendado para 03/05/2024, seguido pelo marco 2 em 07/06/2024 e o marco 3 em 03/07/2024. É fundamental destacar que a documentação correspondente a cada marco deve ser entregue com cinco dias de antecedência em relação à data de apresentação correspondente.</p>

|Marco |Data|  
|------|----|  
|Ponto de controle 1| 03/05/2024|  
|Apresentação do ponto de Controle 1| 08/05/2024|  
|Ponto de controle 2| 07/06/2024|  
|Apresentação do ponto de Controle 2| 12/06/2024|  
|Apresentação| 03/07/2024|  
| FIT | 10/07/2024|  
 
## Tabela de Versionamento

| Data | Versão| Descrição | Autor |   
|------|-------|-----------|-------|   
|29/03/2024|0.1|Estrutura do Termo de Abertura| Miguel|   
|03/05/2024|1.0|Correções e preenchimento | Carla R. Cangussú|  
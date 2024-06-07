# **Arquitetura geral da solução**

## Introdução
<p style="text-align:justify;">O projeto ScanPoint surge como uma resposta à necessidade crescente por soluções que simplifiquem e aprimorem o processo de digitalização 3D e reprodução tridimensional de objetos físicos. Este documento apresenta a arquitetura geral da solução, oferecendo uma visão de alto nível do sistema e detalhando suas principais funcionalidades e componentes.</p>

## Definição do Produto
<p style="text-align:justify;">O ScanPoint é composto por dois principais componentes: uma mesa escaner e um aplicativo desktop. A mesa escaner utiliza um Arduino e sensores infravermelhos para capturar pontos de distância de objetos físicos. O aplicativo desktop permite o acompanhamento do processamento dos pontos e gera um arquivo STL, permitindo o download do modelo e a reprodução do objeto em uma impressora 3D. O foco central do projeto é simplificar e agilizar o processo de digitalização de objetos físicos para posterior impressão em 3D. O objetivo é oferecer uma interface intuitiva que permita a captura eficiente de dados, o processamento otimizado desses dados e a geração de arquivos 3D prontos para impressão. Busca-se estabelecer um sistema robusto e confiável, capaz de realizar o escaneamento com precisão e reproduzir o objeto físico em formato digital.</p>

## Arquitetura Geral da Solução
A arquitetura do ScanPoint é dividida em cinco componentes essenciais:

### Interação com o Usuário
<p style="text-align:justify;">Função: Fornece uma interface intuitiva para o usuário iniciar o processo de digitalização, acompanhar o progresso, cancelar o processo se necessário e pré-visualizar o modelo 3D.
</br>
Design: Interface gráfica desenvolvida no aplicativo desktop, com orientações e feedback em tempo real.</p>

### Captura dos Pontos
<p style="text-align:justify;">Função: Captura os pontos de distância dos objetos físicos usando sensores infravermelhos.
</br>
Design: Utiliza um Arduino conectado aos sensores infravermelhos para coletar os dados de distância. </p>

### Processamento
<p style="text-align:justify;">Função: Processa os pontos capturados para gerar o modelo 3D.
</br>
Design: Algoritmos de processamento no aplicativo desktop convertem os dados de pontos em um modelo 3D, otimizando a geometria para pmais recisão e eficiência.</p>

### Pré-visualização do Resultado
<p style="text-align:justify;">Função: Oferece uma pré-visualização do modelo 3D gerado antes de finalizar o processo.
</br>
Design: Modo de visualização integrado ao aplicativo desktop, permitindo ao usuário inspecionar superficialmente o modelo em 3D e, caso queira, reiniciar o processo.</p>

### Download do Arquivo
<p style="text-align:justify;">Função: Permite ao usuário baixar o arquivo STL gerado para impressão posterior.
</br>
Design: Opção no aplicativo desktop para salvar o arquivo STL, garantindo flexibilidade no uso.</p>

## Considerações de Sustentabilidade
* Eficiência Energética: Projeto de circuitos otimizados para reduzir o consumo de energia.
* Materiais Ecológicos: Compatibilidade com materiais de impressão 3D ecológicos.
* Design Modular: Facilita a atualização e manutenção, prolongando a vida útil do dispositivo.
* Reciclagem: Iniciativa para reciclagem de componentes eletrônicos ao final de sua vida útil.

## Conclusão
A arquitetura do ScanPoint fornece uma visão de alto nível do sistema, destacando suas principais funcionalidades e componentes. Esta abordagem abrangente garante a integração harmoniosa de todas as áreas do projeto, oferecendo uma solução robusta, eficiente e sustentável para a digitalização e reprodução 3D de objetos físicos.

<p style="text-align: justify;"> O detalhamento das arquiteturas específicas podem ser encontrados nos documentos abaixo: </p>

  1. [Software](../software/arquitetura.md);
  2. [Eletrônica](../eletronica-energia/arquitetura_eletronica.md);
  3. [Energia](../eletronica-energia/arquitetura_energia.md);
  4. [Estruturas](../estruturas/arquitetura_subs_estruturas.md);

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 03/04/2024 | Criação do documento de arquitetura geral | Brenda Santos |
| 1.1 | 03/05/2024 | Adição do documento de arquitetura de todas áreas | Pedro Menezes Rodiguero |
| 1.2 | 03/05/2024 | Adicionando arquitetura de energia e eletronica | Brenda Santos |
| 1.3 | 04/05/2024 | Ajustes finais | Ana |
| 2.0 | 07/06/2024 | Ajustes gerais | Brenda |

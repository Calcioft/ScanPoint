# Requisitos gerais

<p style="text-align:justify;"> Os requisitos são peças-chave em qualquer empreendimento, independentemente do campo de atuação, seja ele na área de estruturas, software ou eletroeletrônica. São responsáveis por representar as necessidades, expectativas e limitações a serem consideradas para atingir os objetivos estabelecidos nos projetos. </p>

<p style="text-align:justify;"> Uma distinção comum dentro do escopo dos requisitos é entre **requisitos funcionais** e **requisitos não funcionais**. Os requisitos funcionais descrevem as funcionalidades específicas que o sistema, produto ou serviço deve oferecer. Eles definem as ações que o sistema deve executar, os serviços que ele deve prestar e como ele deve responder às entradas dos usuários. </p>

<p style="text-align:justify;"> Já os requisitos não funcionais dizem respeito às características e qualidades do sistema que não estão diretamente relacionadas às funcionalidades específicas, mas que têm um impacto significativo em sua qualidade global. Isso inclui aspectos como desempenho, segurança, usabilidade, confiabilidade e escalabilidade. </p>

**Requisitos funcionais para o produto**

| Requisito | Nome | Descrição | Observações |
|:---------:| :--- |:---------:|:-----------:|
| RF01 | Captura de pontos do objeto  | O sistema deve ser capaz de capturar os pontos do objeto a ser escaneado com infravermelho. |             |
| RF02 | Rotação constante  | Deve ser possível girar o objeto em uma rotação constante para garantir uma captura uniforme dos pontos do objeto. |             |
| RF03 | Transmissão da nuvem de pontos  | Os pontos do objeto capturados devem ser transmitidos para um computador via cabo USB para processamento posterior. |             |
| RF04 | Processamento de nuvem de pontos  | O software deve processar os pontos recebidos do objeto e gerar um arquivo com formatos de imagem 3D utilizáveis para impressão 3D. |             |
| RF05 | Controle do scanner  | O software deve permitir iniciar e cancelar o processo de escaneamento. |             |
| RF06 | Acompanhamento do escaneamento  | Deve haver uma funcionalidade para acompanhar o progresso do escaneamento em tempo real. |             |
| RF07 | Visualização arquivo 3D  | O usuário deve ser capaz de visualizar (ao terminar o escaneamento) uma *preview* do modelo 3D gerado a partir do objeto |             |
| RF08 | Download arquivo 3D  | O usuário deve ser capaz de baixar (ao terminar o escaneamento) o modelo 3D gerado a partir do objeto |             |
| RF09 | Controle de rotação baseado no peso do objeto  | O usuário deve poder escolher entre 3 velocidades de rotação pré-estabelecidas, mantendo um valor constante de rotação | Deve ser de no máximo 2kg considerando o peso da base e do objeto |

<font size="2"><p style="text-align: center">Tabela 1: Requisitos funcionais</p></font>

**Requisitos não funcionais para o produto**

| Requisito | Nome | Descrição | Observações |
|:---------:| :--- |:---------:|:-----------:|
| RNF01 | Usabilidade do software  | A interface do software deve ser intuitiva e de fácil utilização, permitindo que usuários sem conhecimento técnico possam operá-lo com facilidade.|             |
| RNF02 | Capacidade de carga do motor  | O motor utilizado deve ter capacidade para suportar até 2kg, incluindo a base e o objeto. |             |
| RNF03 | Fixação do infravermelho  | o infravermelho deve ser fixado a uma determinada inclinação para capturar os pontos do objeto de maneira adequada. | O grau precisa ser definido em breve. |
| RNF04 | Alimentação por bateria  | O sistema deve ser alimentado por bateria para garantir sua portabilidade e independência de fontes de energia externas. |             |
| RNF05 | Eficiência de processamento  | O software deve ser eficiente no processamento dos pontos para garantir tempos de resposta aceitáveis durante o escaneamento.  |             |
| RNF06 | Durabilidade e resistência  | Os componentes eletrônicos devem ser selecionados levando em consideração sua durabilidade e resistência às condições ambientais adversas, garantindo uma vida útil prolongada do sistema. | Resistência ao calor e umidade. |
| RNF07 | Design da base | A base deve ser circular, com um diâmetro de 32cm, para acomodar o objeto de forma estável durante o escaneamento. |     |

<font size="2"><p style="text-align: center">Tabela 2: Requisitos não funcionais</p></font>

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 10/04/2024 | Criação do documento | Brenda |
| 1.1 | 30/04/2024 | Atualização dos requisitos gerais| Denniel William |
| 1.2 | 03/05/2024 | Adição do versionamento| Ciro Costa |
| 1.3 | 04/05/2024 | Alteração de alinhamento e fonte | Ana Carolina |


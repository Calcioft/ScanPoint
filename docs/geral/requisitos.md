# Requisitos gerais

Os requisitos são peças-chave em qualquer empreendimento, independentemente do campo de atuação, seja ele na área de estruturas, software ou eletroeletrônica. São responsáveis por representar as necessidades, expectativas e limitações a serem consideradas para atingir os objetivos estabelecidos nos projetos.

Uma distinção comum dentro do escopo dos requisitos é entre **requisitos funcionais** e **requisitos não funcionais**. Os requisitos funcionais descrevem as funcionalidades específicas que o sistema, produto ou serviço deve oferecer. Eles definem as ações que o sistema deve executar, os serviços que ele deve prestar e como ele deve responder às entradas dos usuários. Já os requisitos não funcionais dizem respeito às características e qualidades do sistema que não estão diretamente relacionadas às funcionalidades específicas, mas que têm um impacto significativo em sua qualidade global. Isso inclui aspectos como desempenho, segurança, usabilidade, confiabilidade e escalabilidade.

**Requisitos funcionais para o produto**

| Requisito | Nome | Descrição | Observações |
|:---------:| :--- |:---------:|:-----------:|
| RF01 | Captura de imagens  | O sistema deve ser capaz de capturar imagens do objeto a ser escaneado. |             |
| RF02 | Rotação constante  | Deve ser possível girar o objeto em uma rotação constante para garantir uma captura uniforme das imagens. |             |
| RF03 | Transmissão de imagens  | As imagens capturadas devem ser transmitidas para um computador via cabo USB para processamento posterior. |             |
| RF04 | Processamento de imagens  | O software deve processar as imagens recebidas e gerar um arquivo com formatos de imagem 3D utilizáveis para impressão 3D. |             |
| RF05 | Controle do scanner  | O software deve permitir iniciar e cancelar o processo de escaneamento. |             |
| RF06 | Acompanhamento do escaneamento  | Deve haver uma funcionalidade para acompanhar o progresso do escaneamento em tempo real. |             |
| RF07 | Visualização e Download do Arquivo 3D  | O usuário deve ser capaz de visualizar as imagens capturadas e baixar o arquivo 3D resultante do processo de escaneamento. |             |
| RF08 | Controle de Rotação baseado no Peso do Objeto  | Deve ser possível calcular o nível de força necessário para manter a rotação constante da base, considerando o peso do objeto sobre ela. | Deve ser de no máximo 2kg considerando o peso da base e do objeto |

**Requisitos não funcionais para o produto**

| Requisito | Nome | Descrição | Observações |
|:---------:| :--- |:---------:|:-----------:|
| RNF01 | Usabilidade do software  | A interface do software deve ser intuitiva e de fácil utilização, permitindo que usuários sem conhecimento técnico possam operá-lo com facilidade.|             |
| RNF02 | Capacidade de Carga do Motor  | O motor utilizado deve ter capacidade para suportar até 2kg, incluindo a base e o objeto. |             |
| RNF03 | Fixação da Câmera   | A câmera deve ser fixada a uma determinada inclinação para capturar as imagens do objeto de maneira adequada. | O grau precisa ser definido em breve. |
| RNF04 | Alimentação por Bateria  | O sistema deve ser alimentado por bateria para garantir sua portabilidade e independência de fontes de energia externas. |             |
| RNF05 | Eficiência de Processamento  | O software deve ser eficiente no processamento das imagens para garantir tempos de resposta aceitáveis durante o escaneamento.  |             |
| RNF06 | Durabilidade e Resistência  | Os componentes eletrônicos devem ser selecionados levando em consideração sua durabilidade e resistência às condições ambientais adversas, garantindo uma vida útil prolongada do sistema. | Resistência ao calor e umidade. |
| RNF07 | Design da Base | A base deve ser circular, com um diâmetro de 32cm, para acomodar o objeto de forma estável durante o escaneamento. |     |

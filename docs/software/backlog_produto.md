# Backlog do Produto

O backlog do produto de software pode ser visto como uma lista priorizada de todas as funcionalidades, melhorias e tarefas relacionadas a um produto. Dessa forma, serve como um repositório central para todas as ideias e requisitos do produto, permitindo que a equipe de desenvolvimento e os demais envolvidos gerenciem e planejem o trabalho de forma eficaz. Para isso, o backlog utilizará três principais conceitos: **Épicos** (São itens de alto nível no backlog que representam funcionalidades ou metas de grande escala do produto. São, geralmente, muito amplos e podem não ser facilmente implementados em uma única iteração), **Histórias de usuário** (São unidades menores de trabalho que descrevem funcionalidades ou requisitos específicos do ponto de vista do usuário. Costumam ser mais detalhadas do que épicos e geralmente seguem uma estrutura como "Eu, como [tipo de usuário], quero [realizar uma ação] para poder [atingir um objetivo]") e **Priorização** (Como as histórias e épicos são priorizadas para que o desenvolvimento considere a importância que o cliente dá para cada tópico).

## Priorização - Método MoSCow

Desenvolvida por Dai Clegg durante sua atuação na Oracle na década de 1990, a técnica MoSCoW originou-se no contexto da gestão e dos negócios para aprimorar o processo de desenvolvimento de software. O termo MoSCoW é um acrônimo formado pelas iniciais das categorias "Must Have" (Deve Ter), "Should Have" (Deveria Ter), "Could Have" (Poderia Ter) e "Won't Have" (Não Terá), as quais são utilizadas para segmentar nossas tarefas e determinar suas prioridades:

| Tipo | Descrição |
| :--- | :-------  | 
| Must Have   | “Tem que ser feito” numa tradução literal, seria a categoria para as tarefas mais indispensáveis para o produto, no qual sem elas poderia se considerar um fracasso. |
| Should Have | “Deveria ter”, ou seja, é importante, mas não crucial, por isso são tarefas que devem vir logo após as categorizadas como essenciais.|
| Could Have | “Poderia ter”, tarefas desejáveis, mas que também não necessárias, ou seja, a serem priorizadas apenas se as tarefas das categorias anteriores forem completadas.|
| Won`t Have  | “Não será feito”, tarefas que envolvem muito esforço e têm baixo impacto. Não devem ser priorizadas no momento.|

## Épicos

* **Interface**
* **Captura de Dados em Tempo Real**
* **Escaneamento 3D Automatizado**
* **Interação do Usuário**

### Épico: Interface (E01)
| ID   | Eu, como... | Gostaria de...                                   | Para poder...                                | Priorização |
|------|-------------|--------------------------------------------------|----------------------------------------------|-------------|
| US01 | Usuário     | Iniciar o ScanPoint 3D                        | Começar o processo de escaneamento          | Must Have   |
| US02 | Usuário     | Receber um aviso se o scanner não estiver conectado | Garantir que posso iniciar o escaneamento | Must Have   |
| US03 | Usuário     | Visualizar uma prévia do modelo em nuvem de pontos | Avaliar a qualidade do escaneamento        | Could Have  |
| US04 | Usuário     | Visualizar uma prévia do modelo escaneado       | Confirmar se o escaneamento foi bem-sucedido | Must Have |

### Épico: Captura de Dados em Tempo Real (E02)
| ID   | Eu, como... | Gostaria de...                                   | Para poder...                                      | Priorização |
|------|-------------|--------------------------------------------------|----------------------------------------------------|-------------|
| US05 | Usuário     | Realizar a leitura de objetos em alta definição | Capturar detalhes precisos                          | Must Have   |
| US06 | Usuário     | Escanear os dados através do sensor infravermelho | Garantir precisão no escaneamento                 | Must Have   |
| US07 | Usuário     | Processar os dados recebidos de forma eficiente | Evitar atrasos no escaneamento                    | Must Have   |
| US08 | Usuário     | Transmitir os dados em tempo real para o computador | Acompanhar o progresso do escaneamento         | Must Have   |

### Épico: Escaneamento 3D Automatizado (E03)
| ID   | Eu, como... | Gostaria de...                                   | Para poder...                                      | Priorização |
|------|-------------|--------------------------------------------------|----------------------------------------------------|-------------|
| US09 | Usuário     | Gerar arquivos STL ou G-code precisos e detalhados | Garantir qualidade na impressão                  | Must Have   |
| US10 | Usuário     | Comunicar de forma eficiente com o computador, recebendo dados de status | Acompanhar o progresso do escaneamento | Must Have   |

### Épico: Interação do Usuário (E04)
| ID   | Eu, como... | Gostaria de...                                   | Para poder...                                      | Priorização |
|------|-------------|--------------------------------------------------|----------------------------------------------------|-------------|
| US11 | Usuário     | Ter uma interface para visualizar em tempo real o progresso do escaneamento | Monitorar o processo                              | Could Have  |
| US12 | Usuário     | Fazer o download do arquivo 3D após a conclusão do escaneamento | Uso posterior                                  | Must Have   |
| US13 | Usuário     | Cancelar o escaneamento 3D | Interromper o processo | Must Have  |
| US14 | Usuário     | Reiniciar o escaneamento 3D | começar novamente o processo | Must Have  |

## Referências
* PEREIRA, Paulo; TORREÃO, Paula; MARÇAL, Ana Sofia. Entendendo Scrum para gerenciar projetos de forma ágil. Mundo PM, v. 1, p. 3-11, 2007.

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 28/04/2024 | Criação do documento | Denniel William |
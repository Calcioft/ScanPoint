<!-- Não abordamos 3D -->
## Sistema Inteligente de Captura de Dados e Escaneamento 3D: Requisitos Funcionais e Não Funcionais

### **Introdução**
<!-- Não abordamos 3D -->
O sistema inteligente de captura de dados e escaneamento 3D combina a captura de dados em tempo real com a tecnologia de escaneamento 3D para criar uma solução inovadora para fabricação digital. Este documento apresenta os requisitos funcionais e não funcionais do sistema, que devem ser atendidas para garantir o sucesso do projeto.

### **Requisitos Funcionais**
* **Interface**
    * Iniciar ScannerPoint 3D
    * Checar se o scanner está conectado
    * Visualizar preview do modelo com nuvem de pontos
    * Visualizar preview do modelo escaneado

* **Captura de Dados em Tempo Real:**
    * Realizar leitura de objetos em alta definição;
    * Scannear os dados através do sensor infravermelho;
    * Processar os dados recebidos através do sensor da maneira mais prática e eficiente possível;
    <!-- A principio não faremos a transmissão de dados para a impressora 3D -->
    * Transmissão de dados em tempo real para a computador;
* **Escaneamento 3D Automatizado:**
    <!-- A principio não geramos CAD, geramos stl ou g-code -->
    * Gerar arquivo STL, ou g-code preciso e detalhado a partir da leitura do sensor infravermelho;
    <!-- A princípio não comunicaremos com a impressora -->
    * Comunicação eficiente com a computador, recebendo dados de status do scanner e falhas;

### **Requisitos Não Funcionais**

* **Desempenho:**
    * O tempo de captura de um objeto em alta definição deve ser inferior a X segundos;
    <!-- Não vamos transferir para impressora 3D -->
    * A taxa de transferência de dados entre o sensor e a impressora 3D deve ser superior a Y megabytes por segundo;
    <!-- Não entendi o que seria essa precisão, e não fazemos impressão 3D -->
    * A precisão da impressão 3D deve ser de N por cento.
    <!-- Não fazemos impressão 3D, e tbm não usamos polegadas -->
    * A resolução da impressão 3D deve ser de M pontos por polegadas.
    <!-- Não temos como calibrar os sensores, somente o arduino -->
    * A precisão dos sensores deve ser mantida ao longo do tempo, com calibração regular para garantir medições confiáveis.
* **Usabilidade:**
    * A documentação do sistema deve fornecer instruções claras e concisas para todas as tarefas;
    * A interface do usuário deve ser consistente e de fácil navegação;
* **Confiabilidade:**
    * O sistema deve ser capaz de voltar ao estado inicial caso aconteça algo de errado no scaneamento.
    * O sistema deve ser capaz de sempre gerar um arquivo de nuvem de pontos.
    * O sistema, se requisitado, deve ser capaz de sempre gerar um arquivo .stl.
    * O sistema, se requisitado, deve ser capaz de sempre gerar um arquivo G-code.
* **Compatibilidade:**
    * O Sistema deve ser capaz de ser executado em computadores com arquitetura ARM.
    * O Sistema deve ser capaz de ser executado em computadores com arquitetura AMD64.
    * O Sistema deve ser capaz de ser executado em computadores com arquitetura x86-64.
* **Portabilidade:**
    * O sistema deve ser capaz de ser executado em ambientes com sistema operacional Windows 10 e 11.
    * O sistema deve ser capaz de ser executado em ambientes com sistema operacional MacOs 13 e 14.
    * O sistema deve ser capaz de ser executado em ambientes com sistema operacional linux distribução Ubuntu.
    * O sistema deve ser capaz de ser executado em ambientes com sistema operacional linux distribuição Manjaro.
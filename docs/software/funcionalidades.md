# Funcinalidades

## Introdução

<p align="justify">
O projeto ScanPoint é projetado para fornecer uma solução integrada de captura de dados e escaneamento 3D que transforma objetos físicos em modelos digitais precisos, prontos para impressão 3D. As funcionalidades centrais do sistema foram cuidadosamente delineadas para assegurar a entrega de um produto que não só atenda às expectativas de desempenho técnico mas também ofereça uma experiência de usuário excepcional. A tabela abaixo apresentará as funcionalidades planejadas, cada uma essencial para a operação holística e eficácia do sistema.
</p>

<p align="justify">
A priorização das funcionalidades é crítica para o gerenciamento eficiente do desenvolvimento do projeto e alocação de recursos. Para isso, empregamos o método MoSCoW de priorização, que categoriza as funcionalidades em quatro níveis distintos:
</p>

- **Must have**: Funcionalidades cruciais sem as quais o sistema não pode ser considerado operacional.
- **Should have**: Funcionalidades importantes que agregam valor significativo ao sistema, mas cuja ausência não impede a operação básica.
- **Could have**: Funcionalidades desejáveis que serão implementadas se o tempo e os recursos permitirem, após a implementação das funcionalidades com prioridade mais alta.
- **Won't have this time**: Funcionalidades que reconhecemos como benéficas, mas que não serão implementadas nesta iteração do desenvolvimento, possivelmente devido a restrições de tempo ou orçamento.

<p align="justify">
Cada funcionalidade é acompanhada de uma história de usuário correspondente, expressando os requisitos do ponto de vista do usuário final. Essas histórias guiam nossa equipe de desenvolvimento na criação de soluções que são não apenas tecnicamente sólidas, mas também alinhadas com as expectativas e necessidades reais dos usuários. A tabela de funcionalidades, portanto, serve como um mapa para o desenvolvimento e entrega do projeto.
</p>

## Tabela de Funcionalidades

<font size="2"><p style="text-align: center">Tabela 1: Funcionalidades do sistema ScanPoint 3D</p></font>

| ID da Funcionalidade | Descrição                                                   | Prioridade (MoSCoW) | História de Usuário                                                                                                   |
|----------------------|-------------------------------------------------------------|----------------------|-----------------------------------------------------------------------------------------------------------------------|
| F01                  | Iniciar ScanPoint 3D                                     | Must Have            | Como usuário, quero poder iniciar o ScanPoint 3D para começar o processo de escaneamento.                          |
| F02                  | Checar se o scanner está conectado                          | Must Have            | Como usuário, quero receber um aviso se o scanner não estiver conectado para garantir que posso iniciar o escaneamento. |
| F03                  | Visualizar preview do modelo com nuvem de pontos            | Could Have           | Como usuário, quero poder visualizar uma prévia do modelo em nuvem de pontos para avaliar a qualidade do escaneamento. |
| F04                  | Visualizar preview do modelo escaneado                      | Must Have            | Como usuário, quero poder visualizar uma prévia do modelo escaneado para confirmar se o escaneamento foi bem-sucedido. |
| F05                  | Realizar leitura de objetos em alta definição               | Must Have            | Como usuário, quero que o sistema possa realizar a leitura de objetos em alta definição para capturar detalhes precisos. |
| F06                  | Escanear os dados através do sensor infravermelho           | Must Have            | Como usuário, quero que o sistema possa escanear os dados usando o sensor infravermelho para garantir precisão no escaneamento. |
| F07                  | Processar os dados recebidos através do sensor de forma eficiente | Must Have       | Como usuário, quero que o sistema processe os dados recebidos de forma eficiente para evitar atrasos no escaneamento. |
| F08                  | Transmissão de dados em tempo real para o computador        | Must Have            | Como usuário, quero que os dados sejam transmitidos em tempo real para o computador para acompanhar o progresso do escaneamento. |
| F09                  | Gerar arquivo STL ou G-code preciso e detalhado             | Must Have            | Como usuário, quero que o sistema gere arquivos STL ou G-code precisos e detalhados para garantir qualidade na impressão. |
| F10                  | Comunicação eficiente com o computador, recebendo dados de status | Must Have     | Como usuário, quero que o sistema se comunique de forma eficiente com o computador, fornecendo dados de status atualizados para acompanhamento. |
| F11                  | Fornecer uma interface para visualização em tempo real do escaneamento | Could Have | Como usuário, quero ter uma interface para visualizar em tempo real o progresso do escaneamento para monitorar o processo. |
| F12                  | Permitir o download do arquivo 3D após a conclusão do escaneamento | Must Have  | Como usuário, quero poder fazer o download do arquivo 3D após a conclusão do escaneamento para uso posterior. |
| F13                  | Permitir o usuário cancelar o escaneamento | Must Have  | Como usuário, quero poder fazer o cancelamento do escaneamento 3D para conseguir interromper o processo |
| F14                 | Permitir o usuário reiniciar o escaneamento em caso de falha ou cancelamento | Must Have  | Como usuário, quero poder reiniciar o escaneamento 3D para conseguir começar o processo novamente |

<font size="2"><p style="text-align: center">Fonte: Autoria Própria.</p></font>

## Referências

- [User Stories Applied: For Agile Software Development by Mike Cohn.](https://www.mountaingoatsoftware.com/books/user-stories-applied) Acessado em 29 de abril de 2024

- [Agile Project Management: Creating Innovative Products by Jim Highsmith.](https://www.pearson.com/us/higher-education/program/Highsmith-Agile-Project-Management-Creating-Innovative-Products-2nd-Edition/PGM334840.html) Acessado em 29 de abril de 2024
- [MoSCoW Prioritization](https://www.productplan.com/glossary/moscow-prioritization/#:~:text=MoSCoW%20prioritization%2C%20also%20known%20as,will%20not%20have%20right%20now.) Acessado em 05 de maio de 2024
- [DSDM Project Framework Chapter 10: MoSCoW Prioritization](https://www.agilebusiness.org/dsdm-project-framework/moscow-prioririsation.html) Acessado em 05 de maio de 2024

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 29/04/2024 | Criação do documento | Denniel William |
| 1.1| 03/05/2024 | Refatoração do documento | Pedro Menezes Rodiguero|
| 1.2| 04/05/2024 | Ajuste de alinhamento e fonte | Ana Carolina |

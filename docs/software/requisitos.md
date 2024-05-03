<!-- Não abordamos 3D -->

## Sistema Inteligente de Captura de Dados e Escaneamento 3D: Requisitos Funcionais e Não Funcionais

### **Introdução**

<!-- Não abordamos 3D -->
<p align="justify">
O sistema inteligente de captura de dados e escaneamento 3D combina a captura de dados em tempo real com a tecnologia de escaneamento 3D para criar uma solução inovadora para fabricação digital. Este documento apresenta os requisitos funcionais e não funcionais do sistema, que devem ser atendidas para garantir o sucesso do projeto.
</p>

### Requisitos Funcionais

#### Interface

| Código | Descrição do Requisito                           |
| ------ | ------------------------------------------------ |
| RF01   | Iniciar ScanPoint 3D                          |
| RF02   | Checar se o scanner está conectado               |
| RF03   | Visualizar preview do modelo com nuvem de pontos |
| RF04   | Visualizar preview do modelo escaneado           |

#### Captura de Dados em Tempo Real

| Código | Descrição do Requisito                                            |
| ------ | ----------------------------------------------------------------- |
| RF05   | Realizar leitura de objetos em alta definição                     |
| RF06   | Escanear os dados através do sensor infravermelho                 |
| RF07   | Processar os dados recebidos através do sensor de forma eficiente |
| RF08   | Transmissão de dados em tempo real para o computador              |

#### Escaneamento 3D Automatizado

| Código | Descrição do Requisito                                            |
| ------ | ----------------------------------------------------------------- |
| RF09   | Gerar arquivo STL ou G-code preciso e detalhado                   |
| RF10   | Comunicação eficiente com o computador, recebendo dados de status |

#### Controle de Qualidade

| Código | Descrição do Requisito                                                                 |
| ------ | -------------------------------------------------------------------------------------- |
| RF11   | Verificar a precisão dos dados 3D com relação a parâmetros padrão.                     |
| RF12   | Realizar checagens automáticas de dimensões do objeto antes do escaneamento.           |
| RF13   | Verificar o ângulo do objeto para prevenir distorções no modelo 3D.                    |
| RF14   | Validar todos os processos de escaneamento antes de permitir a impressão do modelo 3D. |

#### Interação do Usuário

| Código | Descrição do Requisito                                                  |
| ------ | ----------------------------------------------------------------------- |
| RF15   | Fornecer uma interface para visualização em tempo real do escaneamento. |
| RF16   | Oferecer uma pré-visualização do modelo 3D para aprovação do usuário.   |
| RF17   | Permitir o download do arquivo 3D após a conclusão do escaneamento.     |

### Requisitos Não Funcionais

#### Desempenho

| Código | Descrição do Requisito                                                       |
| ------ | ---------------------------------------------------------------------------- |
| RNF01  | O tempo de captura de um objeto em alta definição deve ser inferior a 1 hora |
| RNF02  | A qualidade do arquivo de nuvem de pontos deve ser de alta resolução         |
| RNF03  | A precisão do arduino deve ser mantida, com calibrações regulares            |

#### Usabilidade

| Código | Descrição do Requisito                                         |
| ------ | -------------------------------------------------------------- |
| RNF04  | A documentação do sistema deve fornecer instruções claras      |
| RNF05  | A interface do usuário deve ser consistente e fácil de navegar |
| RNF06  | Interface do usuário deve ser intuitiva, mesmo para novos usuários sem experiência prévia em escaneamento 3D. |

#### Confiabilidade

| Código | Descrição do Requisito                                                    |
| ------ | ------------------------------------------------------------------------- |
| RNF07  | O sistema deve poder voltar ao estado inicial se houver falhas no scan    |
| RNF08  | O sistema deve sempre gerar um arquivo de nuvem de pontos, se requisitado |
| RNF09  | O sistema deve sempre gerar um arquivo .stl, se requisitado               |
| RNF10  | O sistema deve sempre gerar um arquivo G-code, se requisitado             |
| RNF11  | O sistema deve ter uma taxa de falha muito baixa em verificações de precisão e checagens de posição. |
| RNF12  | O sistema deve ser capaz de recuperar-se rapidamente de erros de software ou hardware.               |

#### Compatibilidade

| Código | Descrição do Requisito                                                           |
| ------ | -------------------------------------------------------------------------------- |
| RNF13  | O sistema deve ser capaz de ser executado em computadores com arquitetura ARM    |
| RNF14  | O sistema deve ser capaz de ser executado em computadores com arquitetura AMD64  |
| RNF15  | O sistema deve ser capaz de ser executado em computadores com arquitetura x86-64 |

#### Portabilidade

| Código | Descrição do Requisito                                                                                   |
| ------ | -------------------------------------------------------------------------------------------------------- |
| RNF16  | O sistema deve ser capaz de ser executado em ambientes com sistema operacional Windows 10 e 11           |
| RNF17  | O sistema deve ser capaz de ser executado em ambientes com sistema operacional Windows MacOs 13 e 14     |
| RNF18  | O sistema deve ser capaz de ser executado em ambientes com sistema operacional linux distribução Ubuntu  |
| RNF19  | O sistema deve ser capaz de ser executado em ambientes com sistema operacional linux distribução Manjaro |

#### Segurança

| Código | Descrição do Requisito                                                                  |
| ------ | --------------------------------------------------------------------------------------- |
| RNF20  | Assegurar a segurança dos dados transmitidos entre o scanner e o computador/impressora. |

#### Eficiência

| Código | Descrição do Requisito                                                                                                 |
| ------ | ---------------------------------------------------------------------------------------------------------------------- |
| RNF21  | O sistema deve processar e verificar os dados capturados de forma eficiente, minimizando o tempo de espera do usuário. |


## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 0.1 | 26/04/2024 | Criação do documento | Guilherme Basílio e Pedro Menezes |
| 0.2 | 27/04/2024 | Adicionando requisitos não funcionais | Ciro Araújo |
| 0.3 | 27/04/2024 | Adicionando funcionalidades de interface | Denniel William |
| 0.4 | 28/04/2024 | Correção de requisitos não funcionais | Guilherme Basílio |
| 0.5 | 28/04/2024 | Adição de requisitos não funcionais | Vinicius Vieira e Ciro Araújo |
| 1.0 | 29/04/2024 | Formatação das funcionalidades | Denniel William |
| 1.1 | 03/05/2024 | Formatação do documento | Pedro Menezes Rodiguero|

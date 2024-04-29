### Introdução

O projeto ScannerPoint é projetado para fornecer uma solução integrada de captura de dados e escaneamento 3D que transforma objetos físicos em modelos digitais precisos, prontos para impressão 3D. As funcionalidades centrais do sistema foram cuidadosamente delineadas para assegurar a entrega de um produto que não só atenda às expectativas de desempenho técnico mas também ofereça uma experiência de usuário excepcional. A tabela abaixo apresentará as funcionalidades planejadas, cada uma essencial para a operação holística e eficácia do sistema.

A priorização das funcionalidades é crítica para o gerenciamento eficiente do desenvolvimento do projeto e alocação de recursos. Para isso, empregamos o método MoSCoW de priorização, que categoriza as funcionalidades em quatro níveis distintos:

- **Must have**: Funcionalidades cruciais sem as quais o sistema não pode ser considerado operacional.
- **Should have**: Funcionalidades importantes que agregam valor significativo ao sistema, mas cuja ausência não impede a operação básica.
- **Could have**: Funcionalidades desejáveis que serão implementadas se o tempo e os recursos permitirem, após a implementação das funcionalidades com prioridade mais alta.
- **Won't have this time**: Funcionalidades que reconhecemos como benéficas, mas que não serão implementadas nesta iteração do desenvolvimento, possivelmente devido a restrições de tempo ou orçamento.

Cada funcionalidade é acompanhada de uma história de usuário correspondente, expressando os requisitos do ponto de vista do usuário final. Essas histórias guiam nossa equipe de desenvolvimento na criação de soluções que são não apenas tecnicamente sólidas, mas também alinhadas com as expectativas e necessidades reais dos usuários. A tabela de funcionalidades, portanto, serve como um mapa para o desenvolvimento e entrega do projeto.

### Tabela de Funcionalidades

| ID da Funcionalidade | Descrição | Prioridade (MoSCoW) | História de Usuário |
|----------------------|-----------|---------------------|---------------------|
| F01 | Conexão USB com o computador que esta instalado o sistema | Must have | Como usuário, quero que o sistema verifique automaticamente a conexão USB com o computador, para que eu possa iniciar o processo de escaneamento. |
| F02 | Preparação do Objeto | Must have | Como usuário, quero posicionar o objeto na mesa de escaneamento, para que seja escaneado com precisão. |
| F03 | Checagem de peso do objeto | Should have | Como usuário, preciso que o sistema cheque o peso do objeto, para garantir que ele atenda aos requisitos do escaneamento. |
| F04 | Checagem de dimensões do objeto | Should have | Como usuário, quero que o sistema verifique as dimensões do objeto, para assegurar que se ajusta à área de escaneamento. |
| F05 | Escaneamento 3D do objeto | Must have | Como usuário, quero que o sistema escaneie o objeto e crie um modelo digital, para que eu possa utilizá-lo para impressão 3D. |
| F06 | Verificação do escaneamento 3D | Must have | Como usuário, preciso que o sistema verifique a precisão do modelo 3D, para assegurar que é uma réplica exata do objeto físico. |
| F07 | Visualização e correção de erros | Must have | Como usuário, quero visualizar e corrigir quaisquer erros no modelo 3D, para garantir a qualidade antes da geração do arquivo 3D que será utilizado para impressão. |
| F08 | Acompanhamento do escaneamento em tempo real | Should have | Como usuário, quero acompanhar o progresso do escaneamento em tempo real, para monitorar o processo. |
| F09 | Pré-visualização do modelo 3D | Must have | Como usuário, quero pré-visualizar o modelo 3D, para aprovar antes de gerar o arquivo de impressão. |
| F10 | Geração do arquivo de impressão 3D | Must have | Como usuário, quero que o sistema gere o arquivo de impressão 3D, para que eu possa imprimir o objeto físico. |
| F11 | Download do arquivo 3D | Could have | Como usuário, quero ter a opção de baixar o arquivo 3D, para que eu possa armazená-lo ou usá-lo em outro local. |

## Referências

- [User Stories Applied: For Agile Software Development by Mike Cohn. Acessado em 29 de abril de 2024](https://www.mountaingoatsoftware.com/books/user-stories-applied)

- [Agile Project Management: Creating Innovative Products by Jim Highsmith. Acessado em 29 de abril de 2024](https://www.pearson.com/us/higher-education/program/Highsmith-Agile-Project-Management-Creating-Innovative-Products-2nd-Edition/PGM334840.html)
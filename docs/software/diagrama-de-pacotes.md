# Estrutura de Diretórios do Projeto

## `/app`
Raiz do aplicativo, contendo todas as outras pastas e arquivos relevantes para o projeto.

### `/node_modules`
Pasta gerada pelo Node.js que armazena os pacotes de terceiros instalados pelo npm ou yarn. Estes são os módulos de que o aplicativo depende para executar.

### `/src`
Pasta principal que contém o código fonte do aplicativo. 

#### `/types`
Contém as definições de tipos TypeScript para o projeto, facilitando o uso do sistema de tipos do TypeScript para garantir a qualidade do código.

#### `/libraries`
Armazena bibliotecas específicas do projeto ou módulos que podem ser usados em todo o aplicativo.

#### `/services`
Inclui serviços que encapsulam a lógica de negócios, operações de banco de dados, comunicação com APIs externas e qualquer outra funcionalidade central do aplicativo.

#### `/screens`
Específico para arquivos da interface gráfica, esta pasta contém os componentes de tela ou páginas da aplicação.

#### `/components`
Contém componentes reutilizáveis de UI que podem ser usados em diferentes telas ou partes do aplicativo.

### `/assets`
Pasta para armazenar recursos estáticos como imagens e outros arquivos de mídia.

#### `/css`
Armazena arquivos de estilo para o projeto, em formato CSS.

#### `/images`
Contém imagens que serão usadas no aplicativo.

### `/utils`
Pasta para funções utilitárias que fornecem funcionalidades comuns que podem ser compartilhadas em todo o projeto.

## `/tests`
Pasta destinada aos testes do aplicativo, onde são colocados os arquivos de teste que serão executados para validar o comportamento do código.


<iframe frameborder="0" style="width:100%;height:400px;" src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&layers=1&nav=1&title=Diagrama%20de%20Pacotes.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1OZjpVScP9D7Csr7_BQcHX6EjR7xMO650%26export%3Ddownload"></iframe>


## Referências
- [All about UML package diagrams. Acesso em 24 de abril de 2024.](https://www.lucidchart.com/pages/uml-package-diagram)

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 24/04/2024 | Criação do documento | Vinicius Vieira |

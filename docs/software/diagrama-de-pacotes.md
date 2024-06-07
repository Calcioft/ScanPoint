# Estrutura de Diretórios do Projeto

## O que é um Diagrama de Pacotes ?
<p style="text-align:justify;">
Diagramas de pacotes são diagramas estruturais usados para mostrar a organização e disposição de vários elementos de modelo na forma de pacotes. Um pacote é um agrupamento de elementos UML relacionados, como diagramas, documentos, classes ou até outros pacotes. Cada elemento é aninhado dentro do pacote, que é representado como uma pasta de arquivo dentro do diagrama, e então organizado hierarquicamente dentro do diagrama. Diagramas de pacotes são mais comumente usados para fornecer uma organização visual da arquitetura em camadas dentro de qualquer classificador UML, como um sistema de software.
<a href="#ref-1">[1]</a>
</p>

## `/app`
Raiz do aplicativo, contendo todas as outras pastas e arquivos relevantes para o projeto.

### `/node_modules`
Pasta gerada pelo Node.js que armazena os pacotes de terceiros instalados pelo npm ou yarn. Estes são os módulos de que o aplicativo depende para executar.

### `/resources`
Pasta para armazenar recursos estáticos como imagens, fontes, arquivos de configuração e outros arquivos que não fazem parte do código-fonte do aplicativo.

### `/src`
Pasta principal que contém o código-fonte do aplicativo, dividido em três subpastas: main, preload e renderer.

#### `/main`
Contém o código do processo principal do aplicativo, responsável por inicializar o aplicativo e gerenciar os processos de pré-carga e renderização.

#### `/preload`
Contém o código do processo de pré-carga do aplicativo, que é executado antes do processo principal ser carregado e pode ser usado para realizar tarefas como carregar bibliotecas nativas ou interceptar solicitações de rede.

#### `/renderer`
Contém o código da interface gráfica do usuário (GUI) do aplicativo, que é renderizado em uma janela separada do processo principal.

###### `/assets`
Contém arquivos estáticos da GUI, como imagens, CSS e arquivos de configuração.

###### `/components`
Contém componentes reutilizáveis da GUI, como botões, menus e caixas de diálogo.

###### `/screens`
Específico para arquivos da interface gráfica, esta pasta contém os componentes de tela ou páginas da aplicação.

###### `/types`
Contém as definições de tipos TypeScript para o projeto, facilitando o uso do sistema de tipos do TypeScript para garantir a qualidade do código.

###### `/utils`
Pasta para funções utilitárias que fornecem funcionalidades comuns que podem ser compartilhadas em todo o projeto.

## `/tests`
Pasta destinada aos testes do aplicativo, onde são colocados os arquivos de teste que serão executados para validar o comportamento do código.


<iframe frameborder="0" style="width:100%;height:400px;" src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#G1dewdzgdTry6qgIo8Vlwkd4NHWoNoxTGk"></iframe>
<font size="2"><p style="text-align: center">Figura 1: [Diagrama de Pacotes](hhttps://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#G1dewdzgdTry6qgIo8Vlwkd4NHWoNoxTGk).</p></font>

## Referências
<div id="ref-1"/>
- [1][All about UML package diagrams. Acesso em 24 de abril de 2024.](https://www.lucidchart.com/pages/uml-package-diagram)

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 24/04/2024 | Criação do documento | Vinicius Vieira |
| 1.1 | 03/05/2024 | Organização de fontes e referências  | Vinicius Vieira e Ciro Araújo|
| 1.2 | 03/06/2024 | Atualização do diagrama | Guilherme Basilio |
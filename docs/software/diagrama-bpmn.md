# Descrição de processos do Diagrama BPMN 

## O que é BPMN ?
<p style="text-align:justify;">
O Business Process Model and Notation (BPMN) tornou-se o padrão de-fato para diagramas de processos de negócios. Ele é destinado ao uso direto pelos stakeholders que projetam, gerenciam e realizam processos de negócios, mas ao mesmo tempo é preciso o suficiente para permitir que os diagramas BPMN sejam traduzidos em componentes de processos de software. O BPMN possui uma notação semelhante a um fluxograma, fácil de usar e independente de qualquer ambiente de implementação específico.
<a href="#ref-1">[1]</a>
</p>

## 1. Início do Processo:
   
   - O processo começa com um evento de início indicado pelo círculo simples.

## 2. Checagem de Conexão USB:
   
   - Esta etapa verifica se a conexão USB com o computador está estabelecida. Há dois caminhos possíveis:
      - Se a conexão for bem-sucedida, o processo segue para a "Preparação do Objeto".
      - Se houver problemas de conexão, o processo termina, indicado pelo círculo com borda grossa.

## 3. Preparação do Objeto:
   
   - O objeto é preparado para o escaneamento, o que inclui posicioná-lo na mesa de escaneamento.

## 4. Processo de Checagem:
   
   - Este sub-processo, representado por um retângulo com borda pontilhada, contém várias tarefas de verificação:
      - Checagem do comprimento.
      - Checagem da posição.
      - Checagem do ângulo.

   - Após as verificações, existem dois resultados possíveis:
      - Se a checagem for concluída com sucesso, o objeto está preparado, e o processo segue para a etapa "Escanear Objeto".
      - Se houver um problema em alguma das checagens, o processo termina.

## 5. Escanear Objeto:
   
   - O sistema executa o escaneamento 3D do objeto.

## 6. Verificação do Escaneamento:
   
   - O sistema verifica a precisão do escaneamento 3D. Se a verificação for bem-sucedida, o processo passa para o "Acompanhamento do progresso de escaneamento". Se erros forem detectados, segue para a "Visualização dos erros".

## 7. Visualização e Correção de Erros:
   
   - Os erros identificados podem ser visualizados e corrigidos pelo usuário.

## 8. Acompanhamento do Progresso de Escaneamento:
   
   - Esta etapa permite ao usuário acompanhar o progresso do escaneamento.

## 9. Pré-visualização do Arquivo 3D:
   
   - O usuário tem a oportunidade de pré-visualizar o arquivo 3D e, em seguida, aprovar ou não o modelo gerado.

## 10. Geração do Arquivo de Impressão 3D:
   
   - Com a aprovação do usuário, o arquivo de impressão 3D é gerado.

## 11. Download do Arquivo 3D:
   
   - O arquivo de impressão 3D gerado pode ser baixado pelo usuário.

## 12. Fim do Processo:
   
   - O evento de fim é representado pelo círculo com borda grossa.

## Visualização do Diagrama BPMN
<iframe frameborder="0" style="width:100%;height:426px;" src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=BPMN.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1gPlVNqAlODJwvL6Bx6ugGYCwVngh9r1u%26export%3Ddownload"></iframe>

<font size="2"><p style="text-align: center">Figura 1: [Diagrama BPMN](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=BPMN.drawio#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1gPlVNqAlODJwvL6Bx6ugGYCwVngh9r1u%26export%3Ddownload).</p></font>

## Referências

O diagrama BPMN foi construído seguindo as melhores práticas de modelagem de processos de negócios, utilizando o padrão BPMN 2.0. Foi modelado de maneira a oferecer uma visão de ponta a ponta do processo de escaneamento 3D, com ênfase na checagem de pré-requisitos, acompanhamento do usuário e controle de qualidade do objeto digitalizado. Os sub-processos e tarefas foram estruturados para refletir as etapas lógicas do processo, facilitando a compreensão e execução efetiva do escaneamento.
<div id="ref-1" />
- [1][Business Process Model And Notation, acessado em 29 de abril de 2024.](https://www.omg.org/spec/BPMN/2.0/)

## Tabela de versionamento

| Versão | Data       | Descrição                           | Responsável                   |
| ------ | ---------- | ----------------------------------- | ----------------------------- |
| 1.0    | 30/04/2024 | Criação do documento                | Vinicius Vieira e Ciro Araújo |
| 1.1    | 03/05/2024 | Organização de fontes e referências | Vinicius Vieira e Ciro Araújo |



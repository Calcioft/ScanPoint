# Diagrama de Casos de Uso

## O que são casos de uso ?
<p style="text-align:justify;">
Os diagramas de casos de uso em UML são usados durante a fase de requisitos do desenvolvimento de software – eles geralmente colocam os requisitos do sistema em um formato de diagrama, e é fácil ver de relance quais ações um sistema deve suportar. Claro, haverá muitos casos de uso para o seu sistema, e por isso você geralmente precisará desenhar vários diagramas de casos de uso!
<br/>
Junto com outros diagramas UML, como os diagramas de atividade, sequência e componente, os diagramas de casos de uso ajudam você a visualizar seu software e requisitos, antes de mergulhar e começar a programar.
<a href="/software/casos-de-uso#ref-1">[1]</a>
</p>

## 1. Escanear Objeto
- O sistema permite que um usuário escaneie um objeto físico utilizando uma mesa inteligente equipada com sensores. Esta funcionalidade converte a forma, tamanho e características do objeto em um modelo digital.

## 2. Verificação do Escaneamento
- Após o escaneamento, o sistema verifica a precisão dos dados capturados comparando-os com parâmetros pré-definidos, garantindo que o modelo digital de nuvem de pontos seja uma representação fiel do objeto físico.

## 3. Visualização de Erros
- Se erros forem detectados na verificação do escaneamento, o sistema oferece uma interface para que o usuário possa visualizar e corrigir quaisquer discrepâncias antes do escaneamento.

## 4. Checagem de Conexão via USB
- O sistema realiza uma checagem de conexão do sistema com o arduíno via USB, assegurando que haja uma comunicação estável para transferir os dados do modelo.

## 5. Validação do Processo
- Antes de iniciar a checagem do objeto, o sistema verifica se a conexão com o USB foi validado com sucesso.

## 6. Checagem de peso
- Uma balança realiza uma checagem de peso do objeto, assegurando que o peso esteja de acordo com o limite estipulado.

## 7. Checagem do comprimento
- O sensor junto ao Electron (Sistema), realiza uma checagem de comprimento do objeto, assegurando que este esteja em conformidade com as dimensões da mesa.

## 8. Checagem da Posição
- O sistema verifica a posição do objeto em relação à mesa. O objeto deve estar posicionado com uma tolerância de ± 2 mm em relação ao centro da mesa.

## 9. Checagem do Ângulo
- O sistema verifica o ângulo do objeto em relação à horizontal e vertical para garantir que o modelo 3D seja capturado com precisão, sem distorções geométricas.

## 10. Validação do Processo
- Antes de iniciar o escaneamento, o sistema verifica se todos os processos anteriores foram validados com sucesso, garantindo que o modelo esteja pronto para ser escaneado.

## 11. Acompanhamento do Escaneamento
- O usuário pode acompanhar o progresso do escaneamento em tempo real, permitindo uma supervisão detalhada do processo.

## 12. Visualização do Arquivo 3D
- Após a conclusão do escaneamento, o sistema oferece uma pré-visualização do modelo 3D, onde o usuário pode examinar o objeto e aprovar para impressão.

## 13. Geração de Arquivo STL, ou g-code
- Com a aprovação do usuário, o sistema gera o arquivo STL, ou g-code de Nuvem de Pontos adequado, que é salvo no sistema.

## 14. Download do Arquivo 3D
- O sistema também permite ao usuário efetuar o download do arquivo 3D para armazenamento ou uso em outro dispositivo ou local.

## Diagrama abaixo mostra a relação entre os casos de uso:
<iframe frameborder="0" style="width:100%;height:300px;" src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Diagrama%20de%20Casos%20de%20Uso%20-%20Mesa%20Scanner%20-%20PI2#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1zYgIWynN482pM8h9dsHU6t2AOqzia8oi%26export%3Ddownload"></iframe>
<font size="2"><p style="text-align: center">Figura 1: [Diagrama Casos de Uso](https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Diagrama%20de%20Casos%20de%20Uso%20-%20Mesa%20Scanner%20-%20PI2#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1zYgIWynN482pM8h9dsHU6t2AOqzia8oi%26export%3Ddownload).</p></font>

## Referências
<div id="ref-1"/>
- [1][UML use case diagrams with draw.io, acessado em 12 de abril de 2024.](https://drawio-app.com/blog/uml-use-case-diagrams-with-draw-io/)

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 12/04/2024 | Criação do documento | Vinicius Vieira e Guilherme Basílio |
| 1.1 | 27/04/2024 | Atualização do documento | Guilherme Basílio |
| 1.2 | 03/05/2024 | Organização de fontes e referências | Vinicius Vieira e Ciro Araújo |


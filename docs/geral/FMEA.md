# Levantamento de riscos

<p style="text-align:justify;">
Para o levantamento de riscos decidimos utilizar a metodologia FMEA.

O FMEA, ou Análise de Modo e Efeitos de Falha, é uma metodologia usada para identificar e avaliar potenciais falhas em processos, produtos ou sistemas, visando prevenir problemas antes que eles ocorram. Essa técnica é amplamente aplicada em diversos setores, como engenharia, manufatura, saúde e tecnologia, para garantir a qualidade, confiabilidade e segurança dos produtos e processos. Essa metodologia foi escolhida por conta da sua completude de cobertura de anáise de riscos, fazendo análise tanto dos módulos de falha quanto das soluções para evitá-las ou corrigí-las, mitigando seus efeitos.
A análise FMEA envolve uma abordagem sistemática, onde uma equipe multidisciplinar identifica e classifica as possíveis falhas (modo de falha), analisando suas causas e efeitos (efeito da falha), e estimando a gravidade, frequência de ocorrência e detectabilidade de cada falha. Essa análise resulta em uma pontuação de Número de Priorização de Risco (NPR), que permite aos membros priorizar as falhas mais críticas para implementar medidas preventivas ou corretivas.
Além disso, o FMEA é uma ferramenta dinâmica, que pode ser revisada e atualizada ao longo do ciclo de vida dos produtos ou processos, garantindo a contínua melhoria e inovação.
Para o projeto atual, foi feito o seguinte FMEA, conforme tabela abaixo:

</p>
**Tabela 1: FMEA**

| No. | Processo                             | Modo de Falha                                              | Causa da Falha                                         | Efeito da Falha Local                                                | Efeito da Falha Global                       | Severidade | Ocorrência | Detecção | Número de Priorização de Risco (NPR) | Plano de Ação                                                                          | Responsável           | Prevenção                                                                                                                         |
| --- | ------------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------ | -------------------------------------------------------------------- | -------------------------------------------- | ---------- | ---------- | -------- | ------------------------------------ | -------------------------------------------------------------------------------------- | --------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Gestão da Equipe                     | Indisposição de um membro                                  | Problemas pessoais/saúde                               | Sobrecarregar outros membros                                         | Atraso nas atividades                        | 3          | 4          | 1        | 12                                   | Redistribuição das atividades entre membros competentes                                | Gerência              | Comunicação prévia nas reuniões e/ou grupo de conversa                                                                            |
| 2   | Montagem do sistema eletrônico       | Funcionamento inadequado das baterias                      |                                                        | Não fornecimento de energia suficiente aos equipamentos              | Não entrega do projeto por mau funcionamento | 5          | 1          | 1        | 5                                    | Troca da bateria por uma reserva                                                       | Energia               | Testes com as baterias                                                                                                            |
| 3   | Montagem do sistema eletrônico       | Funcionamento inadequado do motor                          | Falta de alimentação/motor quebrado                    | Rotação inadequada da mesa durante a leitura da peça                 | Não entrega do projeto por mau funcionamento | 5          | 1          | 1        | 5                                    | Troca do motor por um motor reserva                                                    | Eletrônica            | Testes com o motor                                                                                                                |
| 4   | Montagem do sistema eletrônico       | Esgotamento da bateria                                     | Mal dimensionamento do tempo de uso                    | Não fornecimento de energia para os equipamentos                     | Não entrega do projeto por mau funcionamento | 5          | 2          | 1        | 10                                   | Troca da bateria por uma reserva                                                       | Energia               | Dimensionar as baterias de acordo com o tempo de funcionamento do projeto e verificar se o tempo é suficiente para a apresentação |
| 5   | Impressão das peças em 3D            | Falta de filamento 3D                                      | Mau cálculo da quantidade de material para a impressão | Estrutura incompleta/Mais tempo para fabricação com outros processos | Atraso na entrega do projeto                 | 3          | 2          | 1        | 6                                    | Uso de outros materiais e processo de fabricação para fazer a estrutura                | Estrutura             | Imprimir com antecedência e revisar o cálculo de quantidade de filamento                                                          |
| 6   | Impressão das peças em 3D            | Falha na impressão                                         | Falta de energia elétrica/problema com a impressora    | Estrutura incompleta/Mais tempo para fabricação com outros processos | Atraso na entrega do projeto                 | 3          | 2          | 1        | 6                                    | Uso de outros materiais e processo de fabricação para fazer a estrutura                | Estrutura             | Imprimir com antecedência e deixar um membro responsável vistoriando a impressão                                                  |
| 7   | Fabricação e Montagem                | Falta de técnicos/Laboratório fechado                      | Greve dos professores e técnicos                       | Impossibilidade de fazer a fabricação e montagem                     | Atraso ou não entrega do projeto             | 5          | 2          | 1        | 10                                   | Encontrar outro local que se possa fazer a fabricação e montagem                       | Estrutura             | Fazer a fabricação e montagem com antecedência                                                                                    |
| 8   | Desenvolvimento de software          | Funcionalidades não entregues                              | Má gestão de tempo da equipe                           | Atraso no progresso de desenvolvimento                               | Não entrega do projeto por mau funcionamento | 3          | 3          | 1        | 9                                    | Redistribuição das atividades entre membros competentes                                | Gerência              | Acompanhamento das atividades e prazos selecionados                                                                               |
| 9   | Desenvolvimento de software          | Drivers incompatíveis                                      | Softwares não compatíveis na mesma plataforma          | Impossibilidade de fazer o desenvolvimento                           | Atraso na entrega do projeto                 | 3          | 2          | 2        | 12                                   | Encontrar novos drivers que consigam trabalhar juntos                                  | Software              | Comunicação prévia nas reuniões e/ou grupo de conversa                                                                            |
| 10  | Desenvolvimento de software          | Bugs incorrigíveis                                         | Plataforma ou bibliotecas com erros incorrigíveis      | Atraso no progresso de desenvolvimento                               | Atraso e/ou não entrega do projeto           | 3          | 1          | 1        | 3                                    | Encontrar formas de contornar os erros, seja por código ou substituição de bibliotecas | Software              | Testes de build da aplicação                                                                                                      |
| 11  | Integração do software com o sistema | Falhas de comunicação dos módulos de software e eletrônica | Conexões ou protocolos                                 | Atraso na Montagem do produto                                        | Atraso e/ou não entrega do projeto           | 5          | 1          | 4        | 20                                   | Fazer uma reunião com os software e de eletrônica para sanar as dificuldades           | Software e eletrônica | Micro testes de integração                                                                                                        |

<font size="2"><p style="text-align: center">Fonte: Tabela Custos - Autoria Própria.</p></font>

Legenda:

- Ocorrência:
    - 1: Muito improvável
    - 2: Ocorre poucas vezes
    - 3: Ocorre ocasionalmente
    - 4: Ocorre frequentemente
    - 5: Sempre ocorre

- Detecção:
    - 1: Detecção garantida
    - 2: Grande chance de detecção
    - 3: Média chance de detecção
    - 4: Pequena chance de detecção
    - 5: Falha não pode ser detectada

- Severidade:
    - 1: Efeito não detectável no sistema
    - 2: Baixa severidade causando aborrecimento leve
    - 3: Severidade moderada: perda de desempenho perceptível
    - 4: Severidade alta com alta insatisfação
    - 5: Severidade muito alta: risco potencial de segurança e problemas graves de não conformidades

<p style="text-align:justify;">
Ao analisar os resultados, destacam-se os problemas identificados com os maiores Números de Priorização de Risco: a falha de comunicação dos módulos de software e eletrônica, classificada com um risco de 20; seguida pela ausência de um membro devido a questões pessoais ou de saúde, com um risco de 12; e, por fim, os desafios apresentados pelos drivers incompatíveis, também com um risco de 12. Esses achados ressaltam a importância de direcionar esforços para mitigar tais questões, visando garantir o sucesso e a eficiência do projeto.
</p>

## Tabela de versionamento

| Versão| Data | Descrição | Responsável|
|-------|------|-----------|------------|
| 1.0 | 13/04/2024 | Criação da tabela de riscos | Diogo Soares, Ciro Costa, Lucas Pantoja  |
| 1.1 | 03/05/2024 | Correção formatação | Artur de Sousa |


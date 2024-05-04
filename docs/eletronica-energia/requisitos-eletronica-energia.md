## Requisitos do Subsistema

<p style="text-align:justify;">
Os requisitos adotados para o subsistema foram selecionados para garantir um funcionamento eficiente, confiável e seguro do scanner de forma que atenda plenamente às necessidades dos usuários.
</p>
<font size="2"><p style="text-align: center">Tabela 1 - Requisitos Funcionais (RF)</p></font>

| Requisito | Nome | Descrição |
|:---------:| :--- |:------------:|
| RF01 | Integração do Motor e Controle de Velocidade | Desenvolver um sistema de controle para o motor da mesa giratória que permita manter a velocidade de rotação e parar a rotação conforme necessário durante o escaneamento do objeto.
| RF02 | Integração do Motor e Altura do Sensor | Desenvolver um sistema de controle para o motor do sistema de regulação de altura do sensor de distância infravermelho.
| RF03 | Comunicação com o Software | Implementar um sistema de comunicação entre o controle dos motores e da iluminação com o software de escaneamento.
| RF04 | Alimentação do Sistema | Projetar um sistema de alimentação elétrica que fornece energia estável e adequada para todos os componentes eletrônicos do scanner, incluindo o motor, sensor de distância infravermelho e circuitos de controle.

<p style="text-align:justify;">
Os requisitos funcionais (RF) abrangem a integração de um motor com o controle de velocidade, permitindo a manutenção e ajuste da velocidade de rotação, bem como a possibilidade de interromper a rotação conforme necessário durante o escaneamento do objeto. Além disso, inclui-se a integração de um segundo motor com o sistema de regulação de altura do sensor de distância infravermelho, assegurando uma adaptação precisa do sensor em relação ao objeto durante o processo de escaneamento. A implementação de um sistema de comunicação entre o controle dos motores e a iluminação com o software de escaneamento também é um requisito funcional crucial. 
</p>

<font size="2"><p style="text-align: center">Tabela 2 - Requisitos Não Funcionais (RNF)</p></font>

| Requisito | Nome | Descrição |
|:---------:| :--- |:------------:|
| RNF01 | Eficiência Energética | Selecionar componentes e desenvolver algoritmos de controle que otimizem o consumo de energia do sistema, maximizando a eficiência energética e minimizando o desperdício de energia.
| RNF02 | Compatibilidade com Normas de Segurança | Seguir as normas de segurança elétrica relevantes para garantir a segurança dos usuários e a conformidade com regulamentações aplicáveis.
| RNF03 | Tempo de Resposta | Garantir um tempo de resposta rápido para as ações de controle do motor, minimizando a latência entre os comandos do software e as alterações na velocidade de rotação da mesa.
| RNF04 | Durabilidade e Confiabilidade | Selecionar componentes de alta qualidade e projetar circuitos robustos para garantir a durabilidade e a confiabilidade do sistema, reduzindo a probabilidade de falhas durante o uso.
| RNF05 | Compatibilidade com Protocolos de Comunicação | Utilizar protocolos de comunicação padrão e amplamente suportados para garantir a interoperabilidade entre os diferentes 

<p style="text-align:justify;">
No que concerne aos requisitos não funcionais (RNF), destaca-se a priorização da eficiência energética para otimizar o consumo de energia do sistema, visando redução de custos operacionais e minimização de desperdício energético. A compatibilidade com normas de segurança elétrica é essencial para assegurar a proteção dos usuários e a conformidade com regulamentações, enquanto a garantia de um tempo de resposta rápido é crucial para uma operação ágil e responsiva do sistema. A durabilidade, confiabilidade e a compatibilidade com protocolos de comunicação são aspectos voltados a promover a estabilidade operacional, maximizando a vida útil do sistema e facilitando a integração entre os componentes eletrônicos.
</p>

## Versionamento

| Versão | Data | Descrição | Responsável |
|-------|------|-----------|------------|
| 0.1 | 21/04/2024 | Adição dos requisitos | Carolina |
| 0.2 | 26/04/2024 | Revisão conforme modificações acordadas pelo grupo | Carolina |
| 0.3 | 03/05/2024 | Adicionando desenvolvimento e corrigindo formatação | Carolina |
| 0.4 | 04/05/2024 | Ajustes de fontes | Ana Carolina |

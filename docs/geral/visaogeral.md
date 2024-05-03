# Documento de Visão

## 1. Introdução

No cenário contemporâneo da fabricação digital, a busca por soluções que simplifiquem e otimizem o processo de digitalização 3D tem sido uma prioridade. Nesse contexto, surge a ideia de desenvolver um scanner 3D a partir de um Arduino, utilizando sensores infravermelho para capturar pontos de distância de objetos físicos. Esses pontos são então enviados para um computador, onde são processados para formar uma nuvem de pontos (point cloud), que por sua vez é utilizada para gerar um modelo tridimensional.

Este projeto representa uma abordagem inovadora e acessível para a digitalização 3D, aproveitando a versatilidade e a capacidade de processamento do Arduino em conjunto com a precisão dos sensores infravermelho. Ao capturar os pontos de distância do objeto em questão, o sistema cria uma representação digital precisa da sua superfície, sem a necessidade de equipamentos complexos ou caros.

Uma vez que os dados são transferidos para o computador, um processo de processamento é acionado para transformar a nuvem de pontos em um modelo 3D completo. Esse modelo pode ser utilizado em uma variedade de aplicações, desde design e prototipagem rápida até engenharia reversa e análise dimensional.

Ao adotar uma abordagem que combina acessibilidade, simplicidade e eficiência, este projeto tem o potencial de democratizar a digitalização 3D, tornando-a acessível a uma ampla gama de usuários, desde entusiastas e estudantes até profissionais e empresas. Além disso, ao utilizar tecnologias de código aberto, incentiva-se a colaboração e o desenvolvimento contínuo, criando um ecossistema de inovação sustentável e compartilhado. Este documento tem como objetivo apresentar o ScanPoint em detalhes, destacando seus recursos, benefícios e aplicações. 

## 2. Definição do Produto

O projeto ScanPoint surge como uma resposta à necessidade crescente de simplificar e otimizar o processo de digitalização e reprodução tridimensional de objetos físicos. Propõe-se a desenvolver um sistema integrado que utilize um Arduino e sensores infravermelho para capturar pontos de distância dos objetos, permitindo sua posterior reprodução em 3D. A motivação para este projeto é proporcionar uma solução abrangente e acessível, desde a captura inicial dos dados até a geração do arquivo 3D pronto para impressão. Ao focar na facilidade de uso e eficiência, o ScanPoint visa democratizar o acesso à tecnologia de digitalização 3D, abrindo portas para a criação e inovação em diversos campos, incluindo design, engenharia e fabricação.

### 2.1. Perspectiva do Produto

O foco central do projeto é simplificar e agilizar o processo de digitalização de objetos físicos para posterior impressão em 3D. O objetivo primordial é oferecer uma interface intuitiva que permita a captura eficiente de dados, o processamento otimizado desses dados e a geração de arquivos 3D prontos para impressão. Em paralelo, busca-se estabelecer um sistema robusto e confiável, capaz de realizar o escaneamento com precisão e reproduzir fielmente o objeto físico em formato digital. Essa abordagem visa não apenas tornar a tecnologia de digitalização 3D mais acessível, mas também garantir resultados de alta qualidade e confiabilidade para uma ampla gama de aplicações.

### 2.2. Resumo dos Recursos

O ScanPoint representa uma solução abrangente para o escaneamento e a reprodução 3D de objetos físicos. Sua abordagem inclui a geração de uma nuvem de pontos precisa, capturando com precisão as características do objeto escaneado. Os recursos foram projetados para garantir uma experiência intuitiva e eficiente, desde a captura inicial dos dados até a criação do modelo 3D pronto para impressão. Para isso, destacam-se cinco componentes essenciais da solução: 
<!-- TODO: [TROCAR AMANHA] -->

* **Interação com o usuário:** Sistema para interação com usuário, dando explicações iniciais necessárias, permitindo iniciar o processo, acompanhar aproximadamente quanto tempo falta até o fim do processo, cancelar e pré-visualizar o resultado do que será enviado para impressão.

* **Captura do objeto:** Realiza a captura de imagens do objeto físico a ser escaneado, garantindo uma rotação constante para obter imagens uniformes. As imagens são transmitidas para um computador via cabo USB para processamento adicional.

* **Processamento:**  O sistema processa as imagens capturadas para gerar um arquivo STL para fatiamento em software de impressão 3D. 

* **Pré visualização do resultado:** Após o processamento das imagens, o sistema oferece uma pré-visualização do resultado final do modelo 3D gerado, permitindo ao usuário revisar e confirmar antes de prosseguir para o download ou a impressão.

* **Download do arquivo:** O usuário tem a opção de baixar o arquivo 3D gerado para impressão posterior, garantindo flexibilidade e conveniência no uso do sistema.

## 4. Restrições

As restrições impostas pelo ScanPoint podem ser críticas para os desenvolvedores e usuários da ScanPoint. Essas limitações podem afetar diretamente a eficácia e a utilidade do equipamento, tornando importante entender e gerenciar esses fatores. Algumas das principais restrições observadas são:

### 4.1. Restrições de Implementação

Considerando as restrições de implementação para o produto "ScanPoint", podemos identificar várias áreas que podem influenciar seu desenvolvimento e produção:

* **Recursos financeiros:** Desenvolver e fabricar uma ScanPoint pode exigir investimentos significativos em pesquisa e desenvolvimento, além de custos associados aos materiais para a construção do scanner. Limitações de orçamento podem influenciar a seleção de materiais, tecnologias e métodos de produção.

* **Tecnologia disponível:** A qualidade da nuvem de pontos gerada pelo ScanPoint pode ser limitada pela precisão dos sensores e algoritmos utilizados na captura dos dados de distância. Restrições relacionadas à resolução e calibração dos sensores podem afetar diretamente a fidelidade e a completude da nuvem de pontos resultante.

* **Materiais:** As restrições relacionadas aos materiais podem incluir a necessidade de selecionar materiais que sejam leves, duráveis e capazes de suportar o peso dos objetos a serem digitalizados. Além disso, os materiais selecionados devem ser compatíveis com as tecnologias de digitalização e não interferir na qualidade dos resultados.

* **Prazos:** Restrições de tempo podem ser impostas por demandas da disciplina para cumprir os prazos estipulados pela ementa e plano de ensino da disciplina, podendo influenciar o escopo e a complexidade do projeto.

### 4.2. Restrições de Uso

Por fim, em relação às principais restrições de uso, podem ser observadas:

* **Tamanho do objeto:** O tamanho máximo do objeto que pode ser testado na ScanPoint é uma restrição significativa. Objetos muito grandes podem não caber na área de digitalização ou podem exceder a capacidade de carga do sistema de rotação, limitando a versatilidade do equipamento.

* **Espessura do objeto:** A espessura máxima do objeto que pode ser digitalizado também é uma restrição importante. Objetos muito finos podem não ser detectados corretamente pelo ScanPoint, resultando em dados imprecisos ou incompletos.

* **Peso do objeto:** A capacidade de carga da ScanPoint define o peso máximo do objeto que pode ser colocado sobre ela. Exceder esse limite pode danificar o equipamento ou comprometer a precisão da digitalização.

* **Tipo de material do objeto:** O tipo de material do objeto a ser testado também pode ser uma restrição. Alguns materiais podem não refletir corretamente a luz do ScanPoint, resultando em dados de baixa qualidade. Além disso, materiais transparentes ou altamente reflexivos podem apresentar desafios adicionais para a digitalização.

## 5. Identificação de solução comerciais
<!-- TODO: [TROCAR AMANHA] -->

| Solução     | Descrição | Principais especificações |
|:------------|------| :------- | 
| Scanner 3D Einscan SE - Shining 3D | O modelo conta com uma mesa giratória que facilita a digitalização 360°C de um objeto e com um "braço" estático que sustenta a câmera responsável pelas capturas das imagens. O resultado da digitalização desse equipamento pode ser exportado nos formatos OBJ, STL e ASC, além da possibilidade de ser processado em aplicações de manufatura aditiva e outros. | Peso máximo do objeto: 5kg, dimensões: 570 x 210 x 210 mm, consumo de energia: 50 W |
| Artec 3D - Artec Turntable | Plataforma giratória inteligente totalmente automatizada e integrada ao software Artec Studio. Alimentado por Bluetooth para digitalização 3D pronta para uso, normalmente é usada para complementar o scanner 3D portátil de ultra-resolução Artec Space Spider.| Peso máximo do objeto: 3kg, dimensões: 250 x 250 x 45 mm, consumo de energia: 12V, 4.66 W |

## 6. Objetivo geral do projeto

O objetivo geral do projeto ScanPoint é desenvolver um sistema integrado que simplifique o processo de escaneamento e reprodução 3D de objetos físicos. O sistema visa oferecer uma solução abrangente que permita aos usuários capturar imagens de objetos do mundo real, processar essas imagens para gerar modelos 3D precisos e, em seguida, criar arquivos prontos para impressão 3D. Por meio do ScanPoint, pretende-se facilitar e agilizar o processo de digitalização de objetos físicos, tornando-o acessível a uma variedade de usuários, desde entusiastas de tecnologia até profissionais de design e fabricação. O sistema busca eliminar as barreiras técnicas e de custo associadas ao escaneamento 3D tradicional, oferecendo uma solução eficiente e fácil de usar.

## 7. Objetivo específicos do projeto

-  **Criação e Aprovação de Protótipo:** Desenvolver um protótipo funcional de alta fidelidade do sistema que o usuário terá contato ao iniciar e acompanhar o processamento. Esse protótipo será projetado para oferecer uma experiência de usuário próxima da realidade, permitindo a validação de conceitos, fluxos de trabalho e usabilidade.

- **Definição da Arquitetura dos Sistemas**: Estabelecer uma arquitetura de software robusta e escalável para o sistema ScanPoint, que permita uma integração eficiente de todos os módulos e componentes. Isso inclui a definição de interfaces de comunicação entre os diferentes subsistemas e a escolha das tecnologias adequadas para implementação.

- **Desenvolvimento dos Sistemas Específicos**: Implementar os sistemas específicos necessários para o funcionamento do ScanPoint, incluindo o sistema de captura de imagens, o sistema de processamento de imagens, o sistema de controle de hardware e o sistema de interface do usuário. Cada um desses sistemas será projetado e desenvolvido de forma a atender aos requisitos específicos do projeto.

- **Testes de Integração**: Realizar testes de integração para garantir que todos os componentes do sistema ScanPoint funcionem harmoniosamente juntos. Isso envolverá a verificação da comunicação entre os diferentes sistemas, a detecção e correção de possíveis conflitos e a garantia de que o sistema como um todo atenda aos requisitos estabelecidos.

- **Validação do Sistema**: Submeter o sistema ScanPoint a testes de validação para garantir que ele atenda aos objetivos e requisitos estabelecidos. Isso incluirá a verificação da precisão do escaneamento, a confiabilidade de hardware e software, e a usabilidade geral do sistema.

- **Documentação**: Preparar documentação detalhada sobre o funcionamento e operação do sistema ScanPoint, bem como materiais de treinamento para usuários e técnicos. Isso garantirá que os usuários estejam devidamente capacitados para utilizar o sistema de forma eficaz e segura.

## 8. Posicionamento

### 8.1. Oportunidade de Negócio

O ScanPoint é um serviço especializado em escaneamento e reprodução 3D de objetos físicos. Nosso objetivo é oferecer uma solução abrangente que simplifique o processo de escaneamento de objetos do mundo real. Com tecnologia avançada e expertise em impressão 3D, a ideia é auxiliar clientes a transformar objetos físicos em modelos digitais precisos. Atendemos diversas necessidades, desde a replicação de peças industriais até a criação de protótipos e obras de arte personalizadas.

### 8.2. Instrução de Posição do Produto

* **Para:** Os cidadãos  
* **Que:**  Desejam ter imagens escaneadas de objetos de pequeno porte
* **O ScanPoint:**  É um aplicativo desktop  
* **Que:** Permite que a população visualize a imagem completa do objeto escaneado e baixe o arquivo gerado
* **Diferente de:** Aplicações similares que não detém de um aplicativo para poder visualizar a imagem e exigem alto custo para fornecer produtos similares 
* **Nosso produto:** Oferece uma visualização com o tempo no qual o objeto está sendo escaneado e permite que o usuário tenha a imagem para enviar a impressora 3D.

### 8.3. Ambiente do Usuário

A aplicação poderá ser acessada por meio de computadores, sendo necessário conexão com a internet apenas para seu download e atualização. Para uso da aplicação não é necessário conexão com a internet, todo o processo de escaneamento, processamento da imagem e geração do arquivo será realizado no ScanPoint e localmente na máquina do usuário.

## 9. Referências

IBM Knowledge Center - Documento de Visão: A estrutura de tópicos do documento de visão. Disponível em: https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_3.0.1/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.htm. Acesso em: 19 mar. 2020;

MIGUEL, Alexandre; ALVES, Dani; GUEDES, Gabriela; GOULART, Helena; ROBSON, João; MENEZES, Leticia; GUILHERME, Luiz; SCHADT, Renan; VINICIUS, Rômulo; HUGO, Victor. Projeto translate.me: Documento de Visão. Disponível em: https://translate-me.github.io/docs/documentos/projeto/doc_de_visao/. Acesso em: 19 mar. 2020;

## 10. Histórico de Revisão

| Data | Versão| Descrição | Autor |
|----|----|----|----|
| 19/04/2024 | 1.0 | Versão inicial do documento com topicos adicionais | Brenda e Ana |
| 23/04/2024 | 2.0 | Ajuste da Introdução, inclusão das soluções comerciais e alteração da instrução de posição do produto | Ana |
| 23/04/2024 | 3.0 | Preenchimento dos tópicos 8.3 ao 8.5, ajustes na formatação e na instrução de posição do produto  | Carla |
| 25/04/2024 | 4.0 | Revisão e ajustes do documento  | Brenda |
| 02/05/2024 | 5.0 | Refatoração dos nomes e explicações  | Ana |

# Projeto do Subsistema de Estruturas

## Materiais

## Definição de critérios de avaliação dos materiais:

Partindo dos requisitos, foram definidos critérios de análise que implicam em sua validação, para cada critério foi avaliado o peso, seguindo sua influência para cada um dos requisitos. Por exemplo, o critério de disponibilidade do material no laboratório recebe um ponto para o requisito de viabilidade econômica como sua veracidade ou não afeta diretamente o custo dos protótipos e do projeto final para o grupo, já o critério de embasamento estrutural literário apresenta nota 0 para esse mesmo requisito pois não gera nenhuma influência sobre os custos do projeto e simultaneamente sobre o requisito RN 1.

Abaixo estão listados os os critérios definidos as pontuações para cada requisito e por fim o peso definido pela soma das pontuações:

| Critério                                    | RF1 | RF2 | RF3 | RF4 | RN1 | RN2 | Peso |
|---------------------------------------------|-----|-----|-----|-----|-----|-----|------|
| Possui normas nacionais para especificar seu uso? |  1  |  1  |  1  |  1  |  0  |  0  |  4   |
| Possui embasamento literário extenso para os cálculos? |  1  |  1  |  1  |  1  |  0  |  0  |  4   |
| Objeto disponível no laboratório?           |  0  |  0  |  0  |  0  |  1  |  1  |  2   |
| Possui vasta aplicação industrial no contexto de estruturas? |  1  |  1  |  1  |  1  |  1  |  1  |  6   |

## Lista e definição de materiais

Após a análise dos requisitos funcionais e não funcionais foi feito um levantamento de materiais disponíveis no laboratório, resultando na seguinte relação:

| Material                                       | Qtd. Disponível |
|------------------------------------------------|-----------------|
| Perfil de alumínio estrutural 20x20mm          |        12       |
| Fuso 8x480mm                                   |        1        |
| Motores de passo                               |        4        |
| Acoplador do motor de passo                    |       ~10       |
| Cantoneiras de alumínio                        |       ~70       |
| Guias de aço 8x600mm                           |        2        |
| Rolamento linear 8mm                           |        2        |
| Suporte de alumínio para eixo linear           |       ~10       |



## Análise Estrutural

texto

### Ensaios Estruturais

Graças aos pontos de restrição a quantidade de normas e trabalhos em peças em impressão 3D, optou-se pela realização de um ensaio para avaliação de integridade estrutural simples onde uma peça de testes foi elaborada e submetida a diversas quantidades de cargas com o intuito de validar seu uso para a aplicação desejada no projeto. A peça em estudo foi fabricada a partir do material PLA (biopolímero ácido poliláctico), com configuração de densidade de preenchimento de 10% do tipo zigue-zague e com 4 paredes de 0,88mm de espessura.

<div align="center">

![Peça utilizada para o ensaio](imagens/Proj_Subs_Estruturas_Ensaios_Peça_analisada_3D.jpg)

<!--<img src="imagens/Proj_Subs_Estruturas_Ensaios_Peça_analisada_3D.jpg" alt="Peça utilizada para o ensaio" width="120" height="120">-->

<!--<img width="100" title="Peça utilizada para o ensaio" src="imagens/Proj_Subs_Estruturas_Ensaios_Peça_analisada_3D.jpg"/> -->

![Geometria de preenchimento da peça](imagens/Proj_Subs_Estruturas_Ensaios_geometria_.jpeg)

</div>


Com o auxílio de um perfil de alumínio e anilhas, a peça foi fixada e submetida continuamente a cargas cada vez maiores. A carga máxima aplicada à peça foi de 51,5 Kg, por não haver possibilidade de acréscimo a esta, não representando sua capacidade máxima de submissão suportada. 

<div align="center">

![Fixação da peça para o ensaio](imagens/Proj_Subs_Estruturas_Ensaios_Fixação_da_peça.jpeg)

![Aparato com aplicação de carga](imagens/Proj_Subs_Estruturas_Ensaios_aplicação_carga.jpeg)

</div>

Como resultado, tem-se que apesar de não ter sido observado o colapso estrutural do material, foram observadas deformações consideráveis na estrutura a partir de 35kg, carga que foi considerada máxima para o retorno da estrutura a suas condições iniciais. Após a definição de um fator de segurança de 2, definindo assim uma carga total por componente impresso de 16kg, calculado da seguinte forma:

<div align="center">

$Fs = \frac{Cf}{Cmax}$

</div>

Onde Fs é o fator de segurança, Cf é a Carga de fratura e Cmax é a Carga máxima admissível considerando o fator de segurança definido.

<div align="center">

![Estrutura da peça após o ensaio](imagens/Proj_Subs_Estruturas_Ensaios_peça_pós_ensaio.jpeg)

![Parafuso de fixação após o ensaio](imagens/Proj_Subs_Estruturas_Ensaios_parafuso_flambado.jpeg)

</div>
 
Assim, avaliando a composição da estrutura com 4 peças impressas em 3D, a carga máxima admissível para o projeto, já considerando o fator de segurança, seria de 64Kg no total, satisfazendo de maneira superdimensionada as condições iniciais e de requisitos do projeto, o que apresenta margem suficiente para simplificação e reduções de rigidez, custos e complexidade dos materiais para as próximas análises de dimensionamentos e de otimização.


### Simulações numéricas

Para complementação e representação do apresentado até então através do ensaio prático estrutural, foi realizada através do software Ansys Workbench uma simulação numérica da peça. 

<div align="center">

![Malha de elementos](imagens/Proj_Subs_Estruturas_Simulação_malha.png)

</div>

Possuindo as mesmas dimensões, a peça foi submetida as condições de contorno de força e apoio, sendo aplicada uma carga de 500N na direção do eixo z e apoios onde a peça foi fixada, considerando as faces em contato com o perfil de alumínio que foi utilizado. Foi determinado, pela limitação do software, um tamanho de malha de 5mm, e foram utilizados 10765 nós e 6447 elementos na mesma.

<div align="center">

![Simulação da deformação da peça](imagens/Proj_Subs_Estruturas_Simulação_deformação.png)

![Face superior da peça real após o ensaio](imagens/Proj_Subs_Estruturas_Ensaios_deformação_face_superior.jpeg)

</div>

Como resultado, tem-se a deformação máxima de aproximadamente 4,84E-05m. Pode-se notar que o resultado mostrou-se visualmente bem próximo ao obtido pelo método anterior e que a deformação ocorre próximo a região de apoio onde foi inserido o parafuso e a ruela para apoio das cargas no objeto em questão.

<div align="center">

![Simulação da deformação total](imagens/Proj_Subs_Estruturas_Vídeo_simulação_deformação_total.mp4)


</div>

# Referências

* KRAJEWSKI, Lee J.; RITZMAN, Larry P.; MALHOTRA, Manoj K. Administração de produção e operações. 8. ed. São Paulo: Pearson, 2012. xiv, 615 p. ISBN 9788576051725.

* ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. ABNT NBR 08403: Aplicação de linhas em desenhos - Tipos de linhas - Larguras das linhas Rio de Janeiro, 1984.

* ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. ABNT NBR 10067 - Princípios Gerais de Representação em Desenho Técnico, 1995

* ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. ABNT NBR 10068 - Folha de Desenho - Leiaute e Dimensões, 1987
 
* ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. ABNT NBR 10126 - Cotagem em Desenho Técnico, 1987



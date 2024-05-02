# Projeto do Subsistema de Estruturas

## Materiais

texto

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


### Simulações e Cálculos Estruturais

texto
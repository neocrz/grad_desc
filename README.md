# grad_desc
O presente repositório contém um estudo sobre a aplicação do gradiente descendente em três situações.
- Regressão polinomial (dados fictícios) `polinomio.ipynb`
- Regressão Logistica `logistica.ipynb`
- Rede Neural `rede_neural.ipynb`

Detalhes de implementação se encontram nos notebooks correspondentes.

## Regressão polinomial
Implementação de um algoritmo para cálculo dos coeficientes de um polinômio de 3º e 17º grau.

## Dados
A implementação da regressão logística e rede neural foram utilizadas no conjunto de dados descrito abaixo.

Os dados utilizados para esse algoritmo foram dados tratados disponibilizados no repositório em outro [projeto](https://github.com/neocrz/heart_disease/tree/main/data) do autor, provenientes primariamente do repositório [45/heart+disease](https://archive.ics.uci.edu/dataset/45/heart+disease) da UC Irvine Machine Learning Repository sob a licensa CC BY 4.0.

### Estrutura
Os dados possuem uma estrutura que pode ser divida entre:
| Var       | Nome               | Função    | Tipo | Descrição                                    | Unidade | Categorias                                                                                  |
|-----------|--------------------|-----------|------|----------------------------------------------|---------|---------------------------------------------------------------------------------------------|
| age       | Idade              | Variável  | Int  | Idade do paciente                            |         |                                                                                             |
| sex       | Sexo               | Variável  | Cat  | Gênero                                       |         | 0: Feminino, 1: Masculino                                                                   |
| cp        | Dor no Peito       | Variável  | Cat  | Tipo de dor no peito                         |         | 1: Angina típica, 2: Angina atípica, 3: Dor não anginosa, 4: Assintomática                 |
| trestbps  | PA em Repouso      | Variável  | Int  | Pressão arterial em repouso                  | mm Hg   |                                                                                             |
| chol      | Colesterol         | Variável  | Int  | Nível de colesterol no soro                  | mg/dL   |                                                                                             |
| fbs       | Glicemia Jejum     | Variável  | Cat  | Glicemia em jejum > 120 mg/dL                |         | 0: Falso, 1: Verdadeiro                                                                     |
| restecg   | Resultados ECG     | Variável  | Cat  | Resultados do eletrocardiograma em repouso   |         | 0: Normal, 1: Anormalidade ST-T, 2: Hipertrofia ventricular esquerda provável              |
| thalach   | FC Máxima          | Variável  | Int  | Frequência cardíaca máxima atingida          | bpm     |                                                                                             |
| exang     | Angina Exercício   | Variável  | Cat  | Angina provocada pelo exercício              |         | 0: Não, 1: Sim                                                                             |
| oldpeak   | Depressão ST       | Variável  | Int  | Depressão do segmento ST pelo exercício      | mm      |                                                                                             |
| slope     | Inclinação ST      | Variável  | Cat  | Inclinação do segmento ST no pico            |         | 1: Ascendente, 2: Plana, 3: Descendente                                                    |
| ca        | Vasos              | Variável  | Int  | Número de vasos principais detectados        |         | 0: 0, 1: 1, 2: 2, 3: 3                                                                     |
| thal      | Condição Cardíaca  | Variável  | Cat  | Tipo de condição cardíaca                    |         | 3: Normal, 6: Defeito fixo, 7: Defeito reversível                                          |
| num       | Diagnóstico        | Alvo      | Cat  | Diagnóstico de doença cardíaca               |         | 0: Sem doença, 1: Doença                                                                   |

Sendo 'num' a variável alvo (resposta) analisada e as demais, as variáveis independentes de entrada.

## Regressão logística
Implementação do algoritmo para regressão logística para obtenção de coeficientes que melhor se ajustem a um conjunto de dados utilizados.

A implementação utiliza a função sigmoide e log loss para ativação e custo da regressão.

## Rede Neural
Implementação do algoritmo para rede neural com apenas uma camada oculta para obtenção de coeficientes que melhor se ajustem a um conjunto de dados utilizados.

A rede neural também utiliza da função sigmoid e log loss como ativação e custo.

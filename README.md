# Maximização da alocação de produtos em espaços tridimensionais

Este repositório contém um projeto de pesquisa sobre a maximização da alocação de produtos em espaços tridimensionais, utilizando duas abordagens diferentes: o método do Simplex e uma heurística baseada no algoritmo genético. O objetivo do trabalho é comparar as soluções obtidas por meio dessas abordagens e analisar sua eficiência na resolução do problema.

## Integrantes

- Erick Henrique Dutra de Souza
- Lucas Cota Dornelas
- Marina Bernardes Diniz

## Professor

Flavio Cruzeiro

## Matéria

Otimização 1 - 2023/1

## Estrutura do Repositório

O repositório está organizado da seguinte maneira:

- `src/`: Este diretório contém o código-fonte dos métodos de solução do problema.
  - `gerando_produtos.ipynb`: Geração de produtos aleatórios para testar as soluções.
  - `containers_solucao.ipynb`: Implementação do método do Simplex e heurística utilizando o algoritmo genético.
- `data/`: Este diretório contém os conjuntos de dados de teste para avaliar as soluções.
  - `products_xxxx.csv`: Conjunto de produtos gerados aleatoriamente.
- `docs/`: Este diretório contém a documentação relacionada ao projeto.
  - `relatorio.pdf`: Relatório final do projeto contendo a descrição do problema, detalhes das abordagens utilizadas, análise dos resultados e conclusões.

## Descrição do Problema

O problema consiste em maximizar o valor dos produtos em N espaços tridimensionais, levando em consideração restrições de volume e capacidade de peso. Dado um conjunto de produtos e um conjunto de espaços disponíveis, o objetivo é determinar a melhor alocação desses produtos nos espaços de forma a maximizar o valor total dos produtos alocados. Cada produto possui um valor, um peso e um volume, e cada espaço possui uma capacidade de peso e um volume.

## Metodologia

O projeto adota duas abordagens para solucionar o problema: o método do Simplex e uma heurística baseada no algoritmo genético.

### Método do Simplex

O método do Simplex é um algoritmo clássico para resolver problemas de programação linear. Nesta abordagem, o problema de alocação de produtos é formulado como um problema de programação linear, e o algoritmo do Simplex é utilizado para encontrar a solução ótima.

### Heurística com Algoritmo Genético

A heurística proposta utiliza o algoritmo genético para encontrar uma solução aproximada para o problema de alocação de produtos. O algoritmo genético é uma técnica de otimização inspirada no processo de evolução biológica. Nessa abordagem, são criadas populações de soluções candidatas, que evoluem ao longo de várias gerações por meio de operadores genéticos, como seleção, crossover e mutação.

## Como Executar

Para executar as soluções implementadas neste projeto, siga as instruções abaixo:

1. Clone este repositório em sua máquina local:

   ```
   git clone https://github.com/lucascdornelas/
   ```

2. Navegue até o diretório `src/`:

   ```
   cd src/
   ```

3. Defina o arquivo de produtos a ser utilizado no método do Simplex e na heurística com o algoritmo genético, alterando o valor da variável `products_file` no arquivo `containers_solucao.ipynb`:

   ```python
   products_file = '../data/products_2000.xlsx'
   ```

4. Execute o arquivo `containers_solucao.ipynb` para utilizar o método do Simplex e a heurística com o algoritmo genético:

   ```
   jupyter notebook containers_solucao.ipynb
   ```

## Resultados

Os resultados obtidos por meio do método do Simplex e da heurística com o algoritmo genético serão apresentados no relatório final do projeto, localizado no diretório `docs/`. O relatório incluirá uma análise comparativa das soluções encontradas, destacando a eficiência e a precisão de cada abordagem.

## Conclusão

Neste projeto de pesquisa, exploramos o problema da maximização da alocação de produtos em espaços tridimensionais. Duas abordagens foram implementadas e comparadas: o método do Simplex e uma heurística baseada no algoritmo genético. Os resultados obtidos demonstraram que o método do Simplex devolve a solução ótima para o problema de forma demorada, enquanto a heurística com o algoritmo genético retorna uma solução aproximada em um tempo muito menor.

Para mais informações, consulte o relatório final do projeto no diretório `docs/`.


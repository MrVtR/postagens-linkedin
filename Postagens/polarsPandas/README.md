# Comparação de Desempenho entre Bibliotecas para Consultas de BigQuery

Este repositório contém um estudo comparativo de desempenho entre as bibliotecas Polars, Pandas-gbq e Pandas para consultas em tabelas do Google BigQuery.
O objetivo principal foi analisar quanto tempo uma amostra de 10 milhões de dados demoraria para ser carregada em memória, simular qual seria o desempenho em uma consulta de 150 milhões de linhas ao considerar uma variação de tempo constante e por fim, criar gráficos comparativos para ver como cada uma se saiu e detectar anomalias também.

## Requisitos

- Python 3.x
- Bibliotecas: `google.cloud`, `google.auth`, `os`, `numpy`, `polars`, `matplotlib`, `datetime` e `time`

## Estrutura do Repositório

- **[Notebook.ipynb](polarsPandas/Analise_Do_Polars_PandasGbq_Pandas_Com_Dados_Do_BigQuery.ipynb)**: Jupyter Notebook contendo o código utilizado na comparação de desempenho.
- **[README.md](polarsPandas/README.md)**: Este arquivo.
- **[LICENSE](LICENSE)**: Licença do repositório.

## Visão Geral do Código

O código utilizado consiste em:

- Importação das bibliotecas necessárias, incluindo `google.cloud`, `google.auth`, `os`, `numpy`, `polars`, `matplotlib`, `datetime` e `time`.
- Estruturação da tabela utilizada nas comparações.
- Definição de funções essenciais para realizar consultas nas bibliotecas estudadas.
- Execução das consultas e comparações de desempenho entre Polars, Pandas-gbq e Pandas.
- Plotagem de gráficos demonstrando o tempo de execução das consultas para análise comparativa.

## Resultados e Conclusões

Os resultados obtidos mostram que o Polars se destacou como a opção mais eficiente entre as três bibliotecas analisadas. Ele foi aproximadamente 20 segundos mais rápido que o Pandas-gbq e quase 50 segundos mais veloz que o Pandas. Esta diferença substancial ilustra a agilidade e eficiência do Polars no processamento de grandes volumes de dados.

Além disso, a capacidade do Polars de converter facilmente entre DataFrames Polars e Pandas oferece flexibilidade aos desenvolvedores, permitindo a escolha da melhor solução para cada desafio específico.

Este estudo destaca a importância de entender  o que cada ferramenta têm a nos oferecer para maximizar a eficiência e desempenho em projetos da engenharia de dados.
Se você também busca eficiência e rapidez na manipulação de grandes conjuntos de dados, o Polars pode ser uma escolha excepcional para usar em conjunto com outras bibliotecas, como o Pandas!

## Contribuição

Fique à vontade para contribuir com sugestões, correções ou melhorias para este estudo comparativo. Sua contribuição é valorizada e pode ajudar a enriquecer ainda mais esta análise.

<a href="#top">🔝 Volte para o topo</a>

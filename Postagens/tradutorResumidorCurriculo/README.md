# Tradutor e Resumidor de Currículo

Este projeto consiste na extração de texto de um currículo em PDF armazenado no Google Cloud Storage (GCS), sua tradução e o resumo do texto em português do Brasil usando o modelo multimodal Gemini-Pro-Vision da Vertex AI.

## Pré-requisitos

Antes de executar o código, certifique-se de ter o seguinte:

- Uma conta do Google Cloud Platform (GCP)
- O Google Cloud SDK instalado
- Bibliotecas: `google-cloud-aiplatform`, `google-cloud-storage`, `PyPDF2`, `os`

## Estrutura do Repositório

- **[Notebook.ipynb](tradutorResumidorCurriculo/tradutor_resumidor_de_curriculos.ipynb)**: Jupyter Notebook contendo o código utilizado na comparação de desempenho.
- **[README.md](tradutorResumidorCurriculo/README.md)**: Este arquivo.
- **[LICENSE](LICENSE)**: Licença do repositório.

## Como usar

1. Crie um bucket do GCS e carregue o arquivo PDF que contém o currículo.
2. Defina as variáveis de ambiente `BUCKET_NAME` e `FILE_NAME` com o nome do bucket e o nome do arquivo PDF, respectivamente.
3. Depois defina as variáveis de ambiente `PROJECT_NAME` e `PROJECT_LOCATION` com o nome do projeto e a localização dele na Google Cloud, respectivamente.
4. Execute o código do Jupyter Notebook.

## O que o código faz?

O código faz o seguinte:

1. Extrai o texto do arquivo PDF armazenado no GCS.
2. Traduz e resume o texto em português do Brasil usando o modelo multimodal Gemini-Pro-Vision da Vertex AI.
3. Imprime o currículo resumido.

## Saída

A saída do código é um currículo resumido em português do Brasil. O resumo contém as seguintes seções:

- Nome do candidato
- Localização
- Introdução
- Habilidades
- Educação
- Experiências prévias
- Certificados
- Experiências voluntárias

## Contribuição

Fique à vontade para contribuir com sugestões, correções ou melhorias para este estudo comparativo. Sua contribuição é valorizada e pode ajudar a enriquecer ainda mais esta análise.

<a href="#top">🔝 Volte para o topo</a>

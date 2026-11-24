# Detecção de arritmias cardíacas por deep learning em aplicação web Python - inferência eficiente em CPU com modelos quantizados treinados em bases públicas de ECG

Projeto de iniciação científica voltado à **detecção de arritmias cardíacas por Deep Learning em sinais de ECG**, com foco em **inferência eficiente em CPU utilizando modelos quantizados**.

## Sobre o projeto

O projeto investiga a possibilidade de treinar modelos de classificação de arritmias em bases públicas de ECG e posteriormente otimizar esses modelos para execução em hardware convencional, sem necessidade de GPU.

São utilizadas as bases:

- **MIT-BIH Arrhythmia Database**
- **PTB-XL**

O projeto contempla todo o pipeline, desde o pré-processamento dos sinais e treinamento dos modelos até a quantização, inferência e disponibilização por meio de uma aplicação web.

## Tecnologias

- Python
- PyTorch
- NumPy / SciPy
- ONNX Runtime
- FastAPI
- Pydantic
- SQLModel / SQLite
- MLflow
- Docker
- Git / GitHub

## Modelos

Serão avaliadas diferentes arquiteturas de Deep Learning para comparação de desempenho e eficiência:

- **1D-CNN** — modelo de linha de base
- **CNN-BiLSTM** — modelo híbrido convolucional e recorrente
- **Modelo otimizado para CPU** — utilizando uma arquitetura com menor custo computacional

O melhor modelo será posteriormente submetido a técnicas de **quantização**, incluindo PTQ e, quando necessário, QAT.

## Inferência

O modelo quantizado será exportado para **ONNX** e disponibilizado através de uma API utilizando **FastAPI**.

A aplicação deverá permitir:

- Classificação de sinais de ECG
- Retorno da classe predita e probabilidades
- Monitoramento da latência de inferência
- Registro de metadados das inferências
- Execução local em CPU

## Avaliação

Além do desempenho de classificação, o projeto avalia a eficiência do modelo em CPU, considerando métricas como:

- F1 macro
- Precisão e sensibilidade
- Matriz de confusão
- Latência
- Throughput
- Consumo de memória
- Tamanho do modelo

O objetivo é analisar o **trade-off entre desempenho diagnóstico e custo computacional**.

> **Aviso:** este projeto possui finalidade acadêmica e experimental. O sistema não constitui dispositivo médico e não substitui avaliação ou diagnóstico realizado por profissional de saúde.

## Estrutura

```text
deteccao-de-arritmia/
├── src/
└── artefatos/
```

## Status

🚧 **Em desenvolvimento**

Projeto desenvolvido no contexto de pesquisa acadêmica em **Inteligência Artificial aplicada à Saúde**, com foco em deployment eficiente de modelos de Deep Learning em CPU.

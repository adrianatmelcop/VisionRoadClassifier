# VisionRoadClassifier

# Classificação de Superfícies de Vias com Visão Computacional

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)

Este repositório contém uma solução de Deep Learning desenvolvida para classificar tipos de pavimentação em vias urbanas e rurais, um componente essencial para sistemas de assistência ao condutor (ADAS) e veículos autônomos.

## 📌 Descrição do Projeto

O objetivo principal é classificar imagens de vias em três categorias distintas:
- **Asphalt (Asfalto)**
- **Belgian Blocks (Paralelepípedo/Blocos de concreto)**
- **Offroad (Terra/Não pavimentado)**

O modelo foi treinado para lidar com variações de iluminação, condições climáticas e diferentes ângulos de captura, utilizando técnicas avançadas de processamento de imagem.

## 🛠️ Tecnologias e Metodologia

- **Arquitetura:** [MobileNetV2](https://arxiv.org/abs/1801.04381) - escolhida pelo excelente equilíbrio entre precisão e eficiência computacional.
- **Transfer Learning:** Utilização de pesos pré-treinados da ImageNet para acelerar a convergência.
- **Validação:** Implementação de **K-Fold Cross-Validation** (5 folds) para garantir a robustez estatística dos resultados.
- **Tratamento de Dados:** - Data Augmentation para reduzir o overfitting.
  - Atribuição de pesos às classes para lidar com o desbalanceamento do dataset.

## 📂 Estrutura do Repositório

```text
├── models/                 # Modelos salvos (.h5 ou .keras)
├── notebooks/              # Jupyter Notebook com todo o pipeline de treino
│   └── DesafioVisaoComputacional.ipynb
├── reports/                # Matrizes de confusão e gráficos de performance
├── requirements.txt        # Bibliotecas necessárias para rodar o projeto
└── README.md               # Documentação do projeto

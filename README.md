# 🌎 Classificação de Imagens de Satélite com Deep Learning

Este projeto explora diferentes técnicas de visão computacional para a **classificação de imagens do UC Merced Land Use Dataset**, utilizando redes neurais convolucionais (CNNs), modelos pré-treinados com Transfer Learning (MobileNetV2, EfficientNetB0, DenseNet121) e embeddings gerados com Vision Transformers (ViT).

## 📁 Estrutura do Projeto

- `CNN simples`: modelo base com 3 camadas convolucionais.
- `Transfer Learning`: aplicação dos modelos MobileNetV2, EfficientNetB0 e DenseNet121 com fine-tuning.
- `Transformers Visuais`: extração de embeddings com ViT e visualização com t-SNE.
- `Modelos Clássicos`: uso de embeddings como entrada para modelos scikit-learn (Logistic Regression, SVM, Random Forest, KNN, Gradient Boosting).
- `Métricas`: precisão, revocação, F1-score e visualização de matriz de confusão.

## 🛰️ Dataset

- **UC Merced Land Use Dataset**  
  - 2.100 imagens (21 classes) de 256x256 pixels  
  - Extraídas do USGS National Map (imagens aéreas urbanas dos EUA)
  - Fonte: [Kaggle](https://www.kaggle.com/datasets/abdulhasibuddin/uc-merced-land-use-dataset)

## 🛠️ Requisitos

- Python 3.8+
- TensorFlow 2.13+
- PyTorch + timm
- scikit-learn
- matplotlib, numpy, PIL
- Google Colab (recomendado para execução com GPU)

## ▶️ Como Executar

1. Suba sua `kaggle.json` no Colab
2. Execute o notebook principal com as células organizadas:
   - Download e pré-processamento
   - Treinamento dos modelos
   - Avaliação e visualização dos resultados

## 📊 Resultados

| Modelo                       | Acurácia |
|-----------------------------|----------|
| CNN Simples                 | 50.6%    |
| MobileNetV2                 | 94.7%    |
| EfficientNetB0              | 95.6%    |
| DenseNet121                 | 95.3%    |
| Regressão Logística (ViT)   | 92.9%    |

## 📚 Referências

- Dosovitskiy et al., 2020 – An Image is Worth 16x16 Words
- Nogueira et al., 2017 – Exploração de CNNs para classificação de cenas remotas
- Sandler et al., 2018 – MobileNetV2
- Tan & Le, 2019 – EfficientNet
- Huang et al., 2017 – DenseNet121
- Van der Maaten & Hinton, 2008 – t-SNE

## 📄 Licença

Este projeto é apenas para fins acadêmicos e de pesquisa. Verifique as licenças dos datasets utilizados.

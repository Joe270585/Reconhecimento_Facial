# Reconhecimento_Facial
Sistema de Reconhecimento Facial em Python (Google Colab)  Este projeto implementa um sistema de reconhecimento facial usando Python, OpenCV e o modelo LBPH (Local Binary Patterns Histograms). O objetivo é treinar o modelo com imagens de diferentes pessoas e depois identificar rostos em novas imagens fornecidas pelo usuário.

📌 Funcionalidades

Treinamento automático com dataset de imagens organizadas por pessoa.

Reconhecimento facial em imagens fornecidas pelo usuário.

Detecção de rostos usando Haar Cascades do OpenCV.

Exibição do nome da pessoa ou "Desconhecido" caso não esteja no dataset.

📂 Estrutura do Projeto
colab_reconhecimento_facial/
│
├── dataset/                # Pasta com imagens para treinamento
│   ├── will_smith/         # 100 imagens do Will Smith
│   ├── robert_downey/      # 100 imagens do Robert Downey Jr
│   └── ...                 # Outras pessoas
│
├── treino.py               # Script de treinamento (LBPH)
├── reconhecimento.py       # Script para reconhecimento em novas imagens
└── README.md               # Documentação


⚠️ Importante: Cada pessoa deve estar em uma pasta separada dentro de dataset/.

⚙️ Instalação

No Google Colab, execute primeiro:

!pip uninstall -y opencv-python opencv-contrib-python
!pip install opencv-contrib-python==4.10.0.84


E depois importe as bibliotecas necessárias:

import cv2
import numpy as np
import os


Possíveis Melhorias Futuras

Substituir o LBPH por uma rede neural (Ex.: FaceNet, Dlib, ArcFace).

Criar uma interface interativa (Streamlit ou Gradio).

Melhorar o pré-processamento das imagens (redimensionamento, alinhamento, normalização).

Implementar reconhecimento em tempo real com câmera.

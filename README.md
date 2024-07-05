# XRay-Chests

XRay Chests é uma prova de conceito e o primeiro contato com modelos de machine learning, o projeto consiste em um código que é capaz de predizer se uma imagem de raio x tem ou não pneumonia e a partir do modelo dizer seu grau de confiança, o modelo foi treinado com um banco de imagens do [kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia?resource=download) e treinado no [teachable machine](https://teachablemachine.withgoogle.com/).

Não existe modelo perfeito e esse se encaixa, mas é funcional e provou que é possível usar IA para fazer análises médicas, o modelo não é definitivo e precisa de muitos outros fatores a se considerar para determinar com confiança a pneumonia. O intuito não é dispensar à necessidade de um profissional da área da saúde mas um pequeno passo para um software que possa democratizar o acesso e ajudar a sociedade.

## Como ele funciona?

O modelo foi treinado usando duas classes (normal e pneumonia), o firmware em python faz a manipulação da imagem e o modelo prediz em qual classe se encaixa.

## Considerações

- O modelo foi treinado na resolução 224x224, não é possivel alterar isso porém a exibição no computador foi pré configurada.
- Imagens fora dessa resolução e com qualidade ruim afeta na acertividade.
- O modelo NÃO DIAGNOSTICA pneumonia e leve isso apenas como uma previsão.

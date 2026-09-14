Reconhecimento de Dígitos Manuscritos com Inteligência Artificial
Mini-Projeto Avaliativo — Módulo 2

Projeto desenvolvido no curso Desenvolvimento de IA para Análise Preditiva — SENAC SCTEC 2026.

Sobre o projeto

Este projeto desenvolve um pipeline de Inteligência Artificial para reconhecimento de dígitos manuscritos utilizando o conjunto de dados MNIST.

O projeto contempla preparação dos dados, análise exploratória, treinamento de modelos, avaliação, análise de erros, generalização e teste com uma imagem manuscrita própria.

Dataset

Foi utilizado o conjunto de dados MNIST.

70.000 imagens
10 classes, de 0 a 9
Imagens em escala de cinza
Resolução de 28 × 28 pixels
784 características por imagem

Os dados foram divididos em:

Treinamento: 56.000 imagens
Validação: 7.000 imagens
Teste: 7.000 imagens

Foi utilizada estratificação para preservar a distribuição das classes.

Modelos utilizados

Foram utilizados três modelos:

K-Nearest Neighbors (KNN)
Random Forest
Multi-Layer Perceptron (MLP)
Avaliação

Os modelos foram avaliados utilizando:

Accuracy
Precision
Recall
F1-score
Classification Report
Matrizes de Confusão
Análise de erros
Tempo de treinamento
Tempo de previsão

Entre as principais confusões observadas esteve a classificação do dígito 4 como 9.

Generalização

Foi realizado um experimento retirando as classes 4 e 7 do treinamento.

Depois, exemplos dessas classes foram utilizados para testar o comportamento dos modelos diante de classes que não estavam presentes no treinamento.

O experimento demonstrou uma limitação importante: quando uma classe não é conhecida durante o treinamento, o modelo tende a classificá-la como uma das classes que conhece.

Teste com imagem própria

Foi realizada uma previsão utilizando uma imagem manuscrita própria.

A imagem passou por preparação para ficar compatível com o MNIST, incluindo:

conversão para escala de cinza;
adequação dos tons;
recorte da região relevante;
centralização;
redimensionamento para 28 × 28 pixels;
normalização;
transformação para 784 características.

A imagem foi submetida aos três modelos treinados.

Tecnologias
Python
Google Colab
NumPy
Pandas
Matplotlib
Scikit-learn
Pillow
Organização do projeto

O projeto foi desenvolvido em seis fases:

Preparação e análise exploratória
Divisão e normalização dos dados
Treinamento dos modelos
Avaliação e comparação
Generalização e classes ocultas
Teste com imagem própria
Arquivos principais
MNIST.ipynb — notebook contendo o desenvolvimento e a execução do projeto.
requirements.txt — bibliotecas utilizadas no projeto.
Uso de Inteligência Artificial

A Inteligência Artificial generativa foi utilizada como ferramenta de apoio durante o desenvolvimento.

Seu uso ocorreu principalmente para compreender conceitos, receber explicações sobre código e bibliotecas, auxiliar na identificação e correção de erros, organizar as etapas e apoiar a documentação do projeto.

A execução do código, os testes no Google Colab e a verificação dos resultados foram realizados durante o desenvolvimento do projeto.

Conclusão

O projeto apresenta um pipeline completo de classificação de dígitos manuscritos utilizando KNN, Random Forest e MLP.

Além da avaliação dos modelos, foram realizados experimentos de análise de erros, generalização para classes não utilizadas no treinamento e previsão de uma imagem manuscrita própria.

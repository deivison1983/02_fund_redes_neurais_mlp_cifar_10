# Implementação de uma Rede Neural Multicamadas (MLP) para Classificação de Imagens no CIFAR-10

## Sobre o projeto

Implementação manual de uma Rede Neural Feedforward com uma camada oculta, incluindo backpropagation e otimização por Gradient Descent, aplicada ao dataset CIFAR-10.

Este projeto apresenta a construção de uma **Rede Neural Artificial Multicamadas (Multi-Layer Perceptron - MLP)**, desenvolvida como parte das atividades do autor em sua Pós-Graduação em Inteligência Artificial e Aprendizado de Máquina.

O objetivo foi desconstruir o funcionamento interno de uma rede totalmente conectada. Para isso, seus componentes essenciais foram implementados utilizando apenas NumPy, sem recorrer a bibliotecas de alto nível como TensorFlow ou PyTorch.

Essa abordagem direta permitiu avaliar, na prática, a mecânica de aprendizado do modelo. O código evidencia o papel crucial da propagação do erro (backpropagation), da otimização baseada em gradientes e do ajuste fino de hiperparâmetros para a criação de sistemas capazes de generalizar novos dados.

Como resultado, o projeto consolida uma base técnica robusta sobre as estruturas matemáticas e os fundamentos algorítmicos que sustentam as arquiteturas modernas de Deep Learning.

---

## Objetivos

Durante esta atividade foram explorados os principais conceitos envolvidos na construção de uma Rede Neural Artificial para classificação de imagens.

Entre os objetivos destacam-se:

- Implementar uma Rede Neural com duas camadas totalmente conectadas (Two-Layer Neural Network);
- Aplicar a função de ativação ReLU;
- Implementar a função de perda Softmax;
- Realizar o cálculo do gradiente por Backpropagation;
- Validar a implementação utilizando Gradient Checking;
- Treinar a rede utilizando o algoritmo Stochastic Gradient Descent (SGD);
- Ajustar hiperparâmetros como taxa de aprendizado, regularização e número de neurônios;
- Avaliar o desempenho do modelo utilizando o dataset CIFAR-10.

Este projeto foi concebido para desmistificar conceitos fundamentais como:

- O fluxo de dados em uma rede fully connected.
- O cálculo manual dos gradientes e a aplicação da **Regra da Cadeia (Chain Rule)**.
- A importância da função de ativação (ReLU) para introduzir não-linearidade.
- O uso da **Validação Cruzada** para escolher hiperparâmetros (learning rate, força de regularização).

---

## Dataset

O projeto utiliza o **CIFAR-10**, uma das bases de dados mais utilizadas em pesquisas de Visão Computacional.

Características do conjunto de dados:

- 60.000 imagens coloridas;
- Resolução de 32 × 32 pixels;
- 10 classes distintas;
- Problema clássico de classificação supervisionada.

Entre as classes presentes encontram-se aviões, automóveis, pássaros, gatos, cervos, cães, sapos, cavalos, navios e caminhões.

---

## Principais Aprendizados e Diferenciais

Este projeto é um "raio-X" das redes neurais, focando nos fundamentos que muitas vezes são abstraídos por bibliotecas modernas:

**Backpropagation Manual:** A implementação da retropropagação (com dout = ...) é o coração do projeto. Calcular os gradientes manualmente para a camada de saída e a camada oculta (ReLU) solidifica o entendimento de como o erro é propagado para trás na rede.

* **Verificação de Gradientes (Gradient Checking):** A utilização da diferença finita para verificar numericamente os gradientes é uma etapa crucial, comum no desenvolvimento de modelos de deep learning, e demonstra uma abordagem profissional de validação de código.

* **Otimização de Hiperparâmetros:** A busca pelos melhores valores de learning_rate e reg (regularização L2) através de uma grade de busca (grid search) com validação cruzada, mostra como ajustar um modelo para melhor generalização.

* **Análise da Função de Perda:** O monitoramento da loss durante o treinamento e a visualização do overfitting quando a regularização é baixa, são aprendizados práticos sobre o comportamento do modelo.

---

## Importância para o Aprendizado em Deep Learning

Embora atualmente existam frameworks capazes de abstrair grande parte da implementação de Redes Neurais, compreender seus mecanismos internos é essencial para o desenvolvimento de soluções robustas em Inteligência Artificial.

Este projeto permite entender como ocorre, passo a passo:

- propagação direta (*Forward Pass*);
- cálculo da função de perda;
- retropropagação do erro (*Backpropagation*);
- atualização dos pesos;
- convergência do treinamento.

Esse conhecimento constitui a base para arquiteturas mais sofisticadas, como:

- Redes Neurais Convolucionais (CNN);
- Redes Recorrentes (RNN);
- LSTM;
- Transformers;
- Modelos de Visão Computacional;
- Grandes Modelos de Linguagem (LLMs).

---

## Tecnologias Utilizadas

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- CIFAR-10

---

## Aplicações

Os conhecimentos desenvolvidos neste projeto são aplicáveis em diversos domínios da Inteligência Artificial, incluindo:

- Classificação de imagens;
- Visão Computacional;
- Sistemas inteligentes;
- Reconhecimento de padrões;
- Desenvolvimento de modelos de Deep Learning;
- Pesquisa em Redes Neurais.

---

## Resultados e Conclusões

A validação de gradientes confirmou que a implementação da backpropagation está correta, com erros relativos muito baixos.

A otimização de hiperparâmetros mostrou que a rede atinge sua melhor performance com um **learning rate moderado e uma força de regularização que equilibra overfitting/underfitting**.

Os gráficos de perda (loss) durante o treinamento ilustram o comportamento típico de convergência, onde a training loss diminui continuamente enquanto a validation loss pode estagnar ou até aumentar se o modelo começar a overfitar.

Este projeto foi fundamental para entender que **redes neurais são otimizadores poderosos, mas altamente dependentes de escolhas de hiperparâmetros**, e que o conhecimento da matemática por trás do algoritmo permite diagnosticar e corrigir problemas de treinamento.

---

## Autor

Deivison Morais. Visite o meu portfólio de projetos [aqui.](https://deivison1983.github.io/portfolio_projetos/)

Pós-Graduação em Inteligência Artificial e Aprendizado de Máquina - PUC Minas

Professor Orientador: Zenilton Patrocínio Jr.

### Contatos

<div>
  <a href = "https://www.linkedin.com/in/deivisonmorais/"><img src = "https://img.shields.io/badge/-deivisonmorais-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href = "mailto:deivison1983@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
</div>

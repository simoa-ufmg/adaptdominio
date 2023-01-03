# Adaptação de domínio
Códigos e experimentos para adaptação de domínio.
Para o desenvolvimento do estudo foi utilizada a linguagem de programação Python versão 3.6, no ambiente de desenvolvimento Google Colaboratory.
#
A falta de grande volude de dados rotulados dos reservatórios no Brasil e a disponibilidade de dados rotulados de outros países justifica o uso de adaptação de domínio. Neste caso, o objetivo foi classificar os valores de turbidez e clorofila com diferentes limiares. Por exemplo, para turbidez foram usados 7, 14 e 25 NTUs como valores limítrofes para as classes 1 e 0.
Apenas os últimos experimentos, com resultados promissores foram incluídos nos subdiretórios. Dentro dos arquivos '.ipynb' situa-se os códigos, a metodologia dos experimentos bem como os resultados alcançados.
# Bibliotecas necessárias
As seguintes bibliotecas são necessárias para a execução do arquivos '.ipynb':
Adapt;
Imbalanced-learn;
Sklearn;
Tensorflow;
Diferentes bibliotecas python para I/O.
 
Arquivos: 'SVMcloro.ipynb ', 'SVMturbi.ipynb ', 'NNcloro.ipynb ' e 'NNturbi.ipynb '
#
Os arquivos são Jupyter Notebook que permite que qualquer pessoa possa fazer o treinamento e a inferência de dois modelos de aprendizado de máquina (SVM e Redes Neurais Artificiais) a partir de um dataset contendo amostras com 12 parâmetros (bandas) de entrada, seu valor de turbidez/clorofila e sua respectiva classe binária determinada a partir dos valores limítrofes tanto para turbidez quanto clorofila.
#
O passo a passo para a execução do Jupyter Notebook é:
1. Carregamento das bibliotecas.
2. Carregamento do dataset.
3. Limpeza, pré-processamento e análise do dataset.
4. Divisão do dataset em subconjuntos de treino e teste:
 4.1. Base USA (Treino e teste mesma base, divisão por longitude)
 4.2. Base USA + Cemig e Cetesb (Treino USA e teste Cemig e Cetesb)
7. Aplicação da técnica SMOTE para aumento de dados (foram realizados experimentos com e sem o aumento de dados)
8. Remoção da feature VALUE que contém o valor de turbidez/clorofila.
9. Separação arquivo de feature e arquivo das classes definidas 
10. Definição dos parâmetros para o método SVM Kernel Polinomial.
11. Treinamento de diferentes modelos de adaptação de domínio para classificação com SVM.
Avaliação e seleção dos melhores modelos obtidos para o método SVM.
Definição dos parâmetros para o modelo de Redes Neurais Artificiais.
Treinamento de diferentes modelos de adaptação de domínio para classificação com redes neurais.
Avaliação e seleção dos melhores modelos obtidos para Redes Neurais Artificiais.


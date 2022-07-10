# Artigo Classificação de sinal ECG

<p align="center">
  <img src="https://user-images.githubusercontent.com/67600860/178149400-19eea358-b3c9-4f8e-8f96-a4cf6a0d767d.png" />
</p>


Este artigo é o trabalho final da disciplina de Redes Neurais do Mestrado em Inteligência Computacional.
Foi proposto aos mestrandos o desafio da aplicação de reses neurais em alguma problemática da vida real. Eu escolhi a aplicação de redes convolucionais aplicadas ao problema de classificação de séries temporais, mais especificamente as séries temporais do sinal de Eletrocardiograma (ECG), pela quantidade de dados disponíveis e estudos prévios na literatura científica.
O modelo foi criado, treinado e avaliado utilizando-se softwares open-source escritos na linguagem de programação Python.
Foram utilizadas, especificamente, as seguintes bibliotecas: Pandas e Numpy para tratamento e modelagem de dados, Matplotlib e
Seaborn para visualização de gráficos, Tensorflow e Keras para criação, treinamento e avaliação do modelo de aprendizagem de
máquina. O código foi escrito utilizando-se o recurso “GoogleColaboratory”.

O artigo pode ser acessado nos arquivos deste repositório e o código pode ser visto neste !link[https://colab.research.google.com/drive/19LsVnQ0sUUyMjtJhDGzL6gmk1ENusJYu?usp=sharing]


#  Resumo

O sinal ECG mede a atividade elétrica do coração e
pode ser usado como medida de monitoramento do sistema
cardiovascular. Neste artigo, é avaliada uma técnica de
classificação de sinais ECG (Eletrocardiograma) em 4 possíveis
classes (Normal, Supraventricular ectopic beat, Ventricular ectopic
beat e Fusion beat), utilizando redes neurais convolucionais (CNN)
a partir de dados do banco MIT-BIH providos pela Physionet.

# Detalhes e implementação

Neste artigo, foi proposto como estudo de caso a utilização de redes neurais convolucionais para classificação de 4 tipos
diferentes de classes relacionadas à arritmias cardíacas, são elas: 
* Normal
* Supraventricular ectopic beat
* Ventricular ectopic beat
* Fusion Beat

Os dados utilizados são provenientes do repositório MIT-BIH (The Massachusetts Institute of Technol-gy - Beth Israel Hospital). Este banco de dados contém 48 gravações de batimentos cardíacos numa taxa de frequência de 360 Hz por aproximadamente 30 minutos de 47 indivíduos diferentes. Cada gravação contém 2 faixas de sinais ECG, sendo a principal delas a faixa A, pois esta contém o complexo QRS de maneira mais proeminente. Cada batimento foi anotado por pelo menos 2 cardiologista, essas anotações foram utilizadas para performar a classificação em cada uma das 4 classes. 

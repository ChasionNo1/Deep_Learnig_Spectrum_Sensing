# Deep Learning for Spectrum Sensing

C�digo utilizado gerar, treinar e avaliar os modelos propostos no artigo.

## Dataset

Os datasets utilizados possuem tamanho em torno de 15 GB. Devido ao tamanho n�o foi poss�vel armazena-los no reposit�rio. 

Os scripts para gerar os datasets est�o dispon�veis na pasta **_generate_dataset** . Depend�ncias necess�rias :

- python 2.7;
- Software GNU Radio com as devidas vari�veis de ambiente apontadas.

## Ambiente

Para rodar os scripts de treinamento e valida��o foram utilizados:

- Python 3.8
- Tensorflow 2.2
- Numpy
- Matplotlib
- Pandas
- Sklearn
- Pickle

## Observa��o

H� uma incompatibilidade ao rodar o modelo DetectNet utilizando o tensorflow CPU devido a camada de convolu��o utilizada. Para contornar esse problema utiliza-se da flag **swap_dim = True** para trocar duas dimens�es do dataset de lugar e assim ser poss�vel executar o script.  

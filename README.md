# Criando Segmentos de Cliente

O projeto faz parte do curso Engenheiro de Machine Learning

![alt text](https://github.com/vyniciuss/NDG_ml_customer_segments/blob/master/segmentos.jpg)

## Visão Geral do Projeto

Neste projeto, irei analisar o conjunto de dados de montantes de despesas anuais de vários clientes (reportados em unidades monetárias), coletados de clientes de uma distribuidora atacadista em Lisboa, para identificar segmentos de clientes ocultos nos dados. Primeiro, irei explorar os dados selecionando um pequeno subconjunto como amostra e determinar se alguma das categorias de produtos está altamente correlacionada com outra. Depois, pré-processarei os dados, dimensionando cada categoria de produto e identificando (e removendo) valores aberrantes. De posse dos dados "limpos", aplicarei PCA a eles e implementarei os algoritmos de clustering para criar os segmentos. Por último, irei comparar a segmentação encontrada com uma marcação adicional, afim de dar ao distribuidor discernimento sobre como melhor estruturar seu serviço de entrega de acordo com as necessidades de cada cliente.

### Dados

O conjunto de dados deste projeto pode ser encontrado no [Repositório de Machine Learning da UCI](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers). Para efeitos de projeto, os atributos 'Channel' e 'Region' serão excluídos da análise – que focará então nas seis categorias de produtos registrados para clientes.

**Atributos**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 
2) `Milk`: annual spending (m.u.) on milk products (Continuous); 
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisbon - 1, Oporto - 2, or Other - 3} (Nominal) 


Este projeto requer **Python 3.6** e as seguintes bibliotecas Python instaladas:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)


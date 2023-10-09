# Projetos de Ciência de Dados Aplicada à Área de Saúde
## Prevendo a Ocorrência de Crises Epiléticas
## Etapa 1 - Definição do Problema
A epilepsia é um distúrbio do sistema nervoso central (SNC), afetando cerca de 1,2% (3,4 milhões de pessoas) nos EUA e mais de 65 milhões em todo o mundo. Além disso, cerca de 1 em cada 26 pessoas desenvolverá epilepsia em algum momento da vida. Existem muitos tipos de convulsões, cada uma com sintomas diferentes, como perda de consciência, movimentos bruscos ou confusão. 

Algumas convulsões são muito mais difíceis de detectar visualmente, os pacientes geralmente apresentam sintomas como não responder ou olhar sem expressão por um breve período de tempo. As convulsões podem ocorrer inesperadamente e podem resultar em lesões como queda, mordedura da língua ou perda do controle da urina ou fezes. Portanto, essas são algumas das razões pelas quais a detecção de convulsões é de extrema importância para pacientes sob supervisão médica que se suspeitem estar propensos a convulsões.

Este projeto usará métodos de classificação binária para prever se um indivíduo está tendo uma convulsão em algum momento.
Objetivo: Prever se um paciente está tendo uma convulsão ou não através de 178 leituras de EEG (Eletroencefalograma) por segundo.
Como métrica de avaliação do modelo usaremos a AUC Score (Area Under The Curve Score), cujo valor vai de 1 a 100% e para esse problema o valor da métrica deve ser aproximadamente de 99%, uma vez que a previsão do modelo está relacionada a casos de vida ou morte. Usaremos a métrica calculada no dataset de validação.

## Etapa 2 - Compreensão dos Dados
O conjunto de dados está disponível no repositório de aprendizado de máquina da UCI e em anexo a este Jupyter Notebook.

https://archive.ics.uci.edu/ml/datasets/Epileptic+Seizure+Recognition

O conjunto de dados inclui 4097 leituras de eletroencefalograma (EEG) por paciente durante 23,5 segundos, com 500 pacientes no total. Os 4097 pontos de dados foram então divididos igualmente em 23 partes por paciente, cada parte é convertida em uma linha no conjunto de dados. Cada linha contém 178 leituras, que são transformadas em colunas; em outras palavras, existem 178 colunas que compõem um segundo das leituras de EEG. No total, existem 11.500 linhas e 179 colunas com a última coluna contendo o status do paciente, esteja ele tendo uma convulsão ou não.

#Limpeza e tratamento de dados usando o Jupyter Notebook

### Em um exame de dados, é normal encontrarmos problemas que possam prejudicar
a fidelidade de um cenário que possamos tentar criar. Esses problemas 
podem ser orginados por vários motivos como:
- operações sem validações, incorrendo em atualizações diretas em banco de dados;
- sistemas antigos;
- inconsistências nos processos de carga:
	- orgigem de informação diversa, não padronizada;
	- mudanças ou erros no processo;
- duplicidade;
- integridade;
- inconformidade;

### O processo de limpeza, análise e tratamento de dados se faz necessário
na coleta de informações para procurar tecer o melhor cenário no que tange a gráficos
na tentativa de retratar a melhor conjuntura que um cenário possa transmitir.

### Este trabalho visa demonstrar de forma sucinta, como podemos fazer isso usando 
as bibliotecas do Python e o Jupyter do Anaconda para tratá-los.

### Informações abaixo descrevem a função em cada campo do código.
<sub>A descrição da função está seguinda de uma cerquilha(#)  e uma In[n], indicando
a linha correspondente.</sub>

###Importação das bibliotecas - In[1]
###Importação dos dados usando a biblioteca Pandas - In[3]
###Visualizando a estrutura do cabeçalho tabela. - In[3]
###Informação sobre a quantidade de linhas e colunas da tabela. - In[4]
###Nomeando as colunas. A forma original da tabela NÃO informa os nomes das colunas. - In[5]
###Visualizando o resultado - In[6]
###Explorando dados categóricos por estados - In[7]
###Visualizando o gráfico dos valores por estados - In[8]
###Agrupando por gêneros masculinos e femininos, informando a quantidade de cada. 
###Esta distribuição será agrupada corretamente. - In[9]
###Visualizando a distribuição dos gêneros - In[10]
###Explorando a coluna 'Score', informando valores conforme descrição à esquerda da tabela. - In[11]
###Gráfico em forma de caixa dos valores apurados na tabela 'Score' - In[12]
###O boxplot demonstra um intervalo de predominância desses valores.
###Gráfico em forma de colunas dos valores apurados na tabela 'Score' - In[13]
###O distplot dispõe uma série de colunas que permite observar as variações dos valores contidos na coluna que desejamos examinar.
###Visão geral dos valores da coluna 'Idade' - In[14]
###Gráfico em forma de bloco, com um intervalo coerente, demonstrando a média de idades e os 'outliers' - valores que fogem do padrão.
###Esses valores serão substituídos pela mediana.
###Erros de digitação. - In[15]
###Informações 'cruas' da coluna 'Saldo'  - In[17]
###Informações 'cruas' da coluna 'Salario' 
###Contagem dos registros nulos - In[23]
###As colunas 'Genero' e 'Salario' contem registros sem valores
###Calculando a mediana na coluna 'Salario' - In[26]
###Substituindo os campos sem registros da coluna 'Salario' pela mediana. - In[27]
###Verificando se há algum valor nulo na coluna 'Salario' - In[28]
###Visualizando o padrão da coluna 'Genero' / esse formato será enxuto.
###Calculando o total de valores nulos na coluna 'Genero' - In[30]
###Preenchendo os valores nulos com a moda(Masculino) - In[31]
###Procurando por valores nulos na coluna 'Genero'
###Padronizando a coluna 'Genero' de acordo com o domínio Masculino e Feminino - In[34]
###Visualizando os dois grupos -In[34]
###Tratando os erros da coluna 'Idade' e redefinindo os valores conforme a mediana. - In[35]
###Visualizar os intervalos de erros.
###Calculando a mediana para substituir os valores que fogem dos padrões - In[37]
###Substituindo os valores errados pela mediana para a coluna 'Idade' - In[38]
###Verificamos se ainda existem idades fora do domínio
###Dados duplicados, buscamos pelo ID - In[40]
###Excluíndo pelo ID - In[41]
###Buscando duplicados 
###Buscando estado fora do domínio  - In[43]
###Atribuindo a MODA para os Estados com erros na digitação ou com pouca expressão no contexto  - In[44]
###Visualizando o resultado
###Usando o desvio padrão para corrigir os valores da coluna 'Salario' que não correspondem ao contexto - In[46]
###Definir padrão como maior que 2 desvios padrão
###Checandos se algum registro atende o critério
###Calculando a mediana para a coluna 'Salario'
###Atualizando os registros dos salarios que tem o valor maior ou igual a duas vezes o desvio padrao pela mediana calculada - In[48]
###Checando alguma pendência para a coluna 'Salario'





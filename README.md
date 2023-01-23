# Notebooks com projetos de data science.
# Projetos:
[Teste_Conhecimento_Tecnico_Bix](#Teste_Conhecimento_Tecnico_Bix)
[Time-Series_Store_Sales_Forecasting](#Time-Series_Store_Sales_Forecasting)

## <a href= 'https://github.com/DorivanKadatzBorba/Notebooks/blob/main/Teste_Conhecimento_Tecnico_Bix.ipynb'> Teste_Conhecimento_Tecnico_Bix.<a>
  (#Teste_Conhecimento_Tecnico_Bix)
  Este projeto era um teste de conhecimento para uma vaga de cientista de dados júnior da empresa Bix, não cheguei a entregar o resultado do meu trabalho, o motivo é a falta de tempo durante o desenvolvimento. Durante o processo seletivo na Gupy, fora entregue um link para a base de dados, até então não estava claro se era uma etapa de perguntas e respostas ou projeto livre, e haveria tempo para a entrega, entrei no link para obter a base de dados e comecei a desenvolver livremente, não dei continuidade no processo seletivo já que eu não tinha uma certeza de quanto tempo seria disposto para entrega do resultado. Gostei da base de dados e me debrucei uns 2 meses testando, modificando, aprendendo e aprendendo, sem me preocupar em dar continuidade no processo seletivo.
  Nesse notebook eu desenvolvi:
  - Fiz uma análise dos dados para conhecer o negócio e assim ter ideias do que desenvolver.
  - A base de dados veio com algumas observações que eu ainda não havia trabalhado antes, dados de vendas do tipo string é um exemplo, fiz então um bom trabalho de limpeza de dados.
  - Fiz um modelo de machine learning não supervisionado para seguimentação de clientes com o algoritimo Kmeans, os clientes foram classificados em 3 clusters e então feito uma análise desses grupos para poder identificar potenciais clientes e suas caracteristicas.
  - Por útimo fiz um modelo de regressão para previsão de vendas com o ARIMA e comparei o desempenho com o XGBoost regressor, o ARIMA funcionou como um modelo base para servir de guia, ainda não tenho tanta experiência com o ARIMA já que esse exige uma curva de aprendizado maior. Para o XGBoost utilize tecnicas de grid search para encontrar os melhores resultados, tanto para os lags quanto para os parâmetros do modelo. Foi feito um reagrupamento dos dados para vendas semanais para uma previsão de 28 semanas(aproximadamente 6 meses de vendas)
  - Os dados represetam uma amostra da rede de lojas de vestuários geek, com dados de vendas, clientes, produtos. Em suma, tratei os dados como total, apenas na etapa de análise de dados eu analisei as lojas separadamente.
  - No total temos 22 meses de dados, são 6 lojas situadas em estados diferentes e uma loja online.
  - O conjunto de dados de vendas tem uma média de 77473.41 e desvio padrão 21815.81 para a rede de lojas somados.
  - O resultado final do XGBoost regressor ficou:
    - MAPE(Erro percentual médio, nada mais é do que uma medida em porcentagem do quanto o modelo erra em relação aos dados reais): 18.77%
    - R2(Coeficiente de determinação, representa o quão próximos os dados estão da linha de regressão ajustada): 0.59
    - MAE(Erro absoluto médio, é a media absoluta dos erros): 12648.7
    - RMSE(Raiz quadrada média dos erros, é uma métrica utilizada por ser sensível aos erros maiores): 15415.63
Em resumo, o modelo de previsão errou em média aproximadamente 19% para cima ou para baixo em relação ao valor verdadeiro.

# <a href= 'https://github.com/DorivanKadatzBorba/Notebooks/blob/main/time-series-store-sales-forecasting.ipynb'>Time-Series_Store_Sales_Forecasting.<>
(#Time-Series_Store_Sales_Forecasting)
  Este foi meu primeiro projeto utilizando dados disponibilizado na plataforma kaggle, uma competição de data science com o propósito de prever vendas de produtos, os dados são de uma rede de supermercados do Equador denominada Corporación Favorita. Os dados já estavam tratados sendo apenas necessário pular direto para o desenvolvimento do modelo.
  A plataforma kaggle tem forte predominância no inglês como linguagem, o que não é de se espantar, portanto mantive a mesma linguagem durante o desenvolvimento do notebook afim de também aprimorar meu inglês.
  A competição tinha como premissa prever a venda de produtos para cada loja da corporação, e então subir o resultado para avaliação da plataforma.
  Utilizei o XGBoost regressor, um modelo supervisionado de machine learning de regressão baseado em arvore de decisões impulsionada por gradiente.
  - O resultado do modelo foi um desastre, já que, foi minha primeira tentativa com o algorítimo, irei retornar ao projeto e refaze-lo futuramente.
  Apesar de não ter conseguido um bom resultado, garantiu meu aprendizado e consistência. a partir desse projeto, pude aprender e pesquisar por soluções a qual eu não fazia com os dados padrões de aprendizado como por exemplo o Iris, que já tem milhares de soluções por aí.
  Manterei o notebook mesmo com péssimo resultado até sua próxima atualização, é o resultado de um estudante que erra, tenta e aprende como qualquer pessoa comum no ato de estudar.

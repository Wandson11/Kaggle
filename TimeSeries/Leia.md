 Curso do kaggle para elaboracao de maquina de aprendizado aplicado em series temporais. Ao todo são 06 modulos: https://www.kaggle.com/learn/time-series
 01 - fala de etapa de tempo e de recursos de atrasos, ambos aplicados na regressão linear.
 - uso do time dummy: variavel (recursos de passo de tempo), serve para criar algo pareicdo com um indice indo de zero até o último elemento = np.arange(len(df.index))
 - Uso do shift para lag feature (recurso de atraso) ou diferença de um dia para o outro: lag_1 = df['sales'].shift(1)
 02 - fala em calcular a mudança da média com estimativas de tendencia/ criação de tendencia via deterministiProcess
 - Uso de coluna.rolling().mean() para apurar a média de n dias (a quantidade de dias será inclusa dentro dos parênteses.)
 - Para criar a tendencia existem 3 passos: deterministprocess(), criar conjunto de recursos para as datas: "variavel que recebeu o deterministprocess".in_sample(); criando a previsão de dias: "variavel da deterministprocess".out_of_samples(steps=x dias)

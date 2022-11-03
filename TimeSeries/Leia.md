 Curso do kaggle para elaboracao de maquina de aprendizado aplicado em series temporais. Ao todo são 06 modulos: https://www.kaggle.com/learn/time-series
 01 - fala de etapa de tempo e de recursos de atrasos, ambos aplicados na regressão linear.
 - uso do time dummy: variavel (recursos de passo de tempo), serve para criar algo pareicdo com um indice indo de zero até o último elemento = np.arange(len(df.index))
 - Uso do shift para lag feature (recurso de atraso) ou diferença de um dia para o outro: lag_1 = df['sales'].shift(1)

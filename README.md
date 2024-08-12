# Realized-volatility-ML
Il seguente progetto è basato sulla challenge kaggle [Optiver Realized Volatility Prediction](https://www.kaggle.com/competitions/optiver-realized-volatility-prediction)

La volatilità dei mercati finanziari rappresenta una misura fondamentale del rischio e dell'incertezza associati ai prezzi degli asset.

La volatilità realizzata è una misura della variabilità dei rendimenti di un asset nel tempo. Più specificamente, essa viene calcolata come la deviazione standard dei rendimenti di un asset durante un determinato periodo di tempo.


L'obiettivo è sviluppare un modello che in grado di stimare la volatilità realizzata per diverse azioni con un orizzonte temporale di 10 minuti, utilizzando *order book* e *trade log* dei precedenti 10 minuti.
Il modello inoltre dovrà predire solo risultati sulle azioni usate in fase di training

La challenge fornisce un dataset di training e prevede la submission del notebook per la valutazione con un dataset "nascosto" (con la garanzia di mantenere le stesse azioni utilizzate nel training, questo ci permette quindi di utilizzarle come parametro per il training). Non avendolo a disposizione si opterà per dividere il training set "originale" in un training set e un validation set, questo è possibile anche grazie alla grande quantità di dati disponibili nel dataset originale.  

# Tweets_classification_RNN
Решается задача классификации твитов (реальный vs фейковый твит) с использованием рекуррентных нейросетей (LSTM, GRU, LSTM and GRU)

Файлы train.csv и test.csv содержат данные формата pd.DataFrame([['text', 'label']]), если считывать библиотекой pandas.
В тетрадке disaster_tweets_classification_ANALYTICS.ipynb проводится предварительная аналитика текстов в выборке.
В тетрадках disaster_tweets_classification_LSTM.ipynb, disaster_tweets_classification_GRU.ipynb, disaster_tweets_classification_LSTM_and_GRU.ipynb проводится обучение LSTM, GRU, LSTM и GRU архитектур соответственно. В качестве библиотеки использовался PyTorch. Модель представляла из себя слои Embedding (для векторного представления слов в тексте), LSTM/GRU слои для преобразования всех векторов в единный вектор, учитывающий весь его контекст от начала до конца, Linear слой для преобразования итоговых векторов в вероятность принадлености текста классу 1.

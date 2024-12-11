# VEGA [Программная инженерия С++]
Цель проекта:
Разработать модель прогнозирования спроса (продаж) товаров в одном из магазинов офлайн-ритейлера в США на три временных интервала: неделю, месяц и квартал. Основная задача — реализовать класс для обучения, оценки и предсказания спроса с использованием классических методов временных рядов.

Ключевые задачи:

Предобработка данных: Подготовка данных в удобный формат для анализа и моделирования (учет сезонности, влияния цен и праздников).

Построение моделей: Использование классических моделей временных рядов (например, ARIMA, Exponential Smoothing, Seasonal Decomposition).

Оценка качества: Прогнозирование продаж на указанные интервалы с последующей оценкой точности на тестовом наборе данных с помощью метрик MAE, RMSE и MAPE.

Визуализация: Построение графиков прогнозов и сравнение их с фактическими данными.

Вывод: prophet показал себя лучше других моделей на предсказаниии на недлительный период (7 дней). На более длительных периодах prophet хорошо работает только на данных с чётко выделенной сезонностью, а на данных без четкой структуры лучше STL. naiv тоже показывает довольно неплохие результаты на длительном периоде. Лучшая достигнутая метрика MAE = 0.648543, а лучшая метрика MAPE = 1.860501e-01, обе получены для предсказания на 7 дней модели prophet.

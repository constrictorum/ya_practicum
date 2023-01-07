# Описание проекта

Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час. Постройте модель для такого предсказания.

Значение метрики RMSE на тестовой выборке должно быть не больше 48.

# Инструкция по выполнению проекта

- Загрузите данные и выполните их ресемплирование по одному часу.
- Проанализируйте данные.
- Обучите разные модели с различными гиперпараметрами. Сделайте тестовую выборку размером 10% от исходных данных.
- Проверьте данные на тестовой выборке и сделайте выводы.

# Описание данных

Данные лежат в файле /datasets/taxi.csv. [Скачать датасет](https://code.s3.yandex.net/datasets/taxi.csv).

Количество заказов находится в столбце 'num_orders' (от англ. number of orders, «число заказов»).
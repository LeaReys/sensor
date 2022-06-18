# Water Рump Maintenance

## Описание задачи:
В качестве исследуемых  данных используется набор показаний датчи-ков для профилактического обслуживания водяного насоса: https://www.kaggle.com/datasets/nphantawee/pump-sensor-data?datasetId=131138&sortBy=voteCount

Описание данных на  «Kaggle»: «Один из водяных насосов системы во-доснабжения отказывал 7 раз, что ведет к полной остановке системы.  Инженеры не заметили никакой закономерности в данных при сбоях системы, поэтому предоставили показания датчиков, для разработки системы обнаруже-ния аномалий».

Массив исследуемых данных представляет показания 52 датчиков за определенный временной период, а также столбец, который содержит текстовые логи о состоянии системы.

**Постановка задачи:**  построить модель машинного обучения, которая будет детектировать «ненормальное» поведение системы за 24 часа до отказа. Процесс обнаружения аномалий состоит из ввода данных в модель, получение вектора с предсказанными аномалиями и сравнение с целевым вектором.

Задача является случаем предсказания обслуживания, а именно размет-кой аномального поведения. Для решения поставленной задачи используются методы обучения без учителя: KMeans, LOF, iForest, OCSVM. 


## Файлы:

Подробные выводы и рассуждения в формате PDF: https://drive.google.com/file/d/1xj0BrH2guPJihJ8Z_UeZ45VizmDXCyO0/view?usp=sharing.
В данный PDF-файл является частьью моего дипломного проекта, в файле приводятся развернутые рассуждения и выводы касательно выбранных подходов и полученных результатов, а также сравнение показателей метрик.

**Архив со всеми файлами**: https://drive.google.com/file/d/1L2A-eZC061cCLrCDt35Rv6NVsrr--1XO/view?usp=sharing

**Порядок файлов:**
1. sensor_ml_part_1 - Первичный анализ данных
2. sensor_ml_part_2 - Предобработка данных
3. sensor_ml_part_3_IQR - Модель доверительного интервала IQR
4. sensor_ml_part_3_iForest - Модель изоляционного леса
5. sensor_ml_part_3_Kmean - Модель KMeans
6. sensor_ml_part_3_LOF - Модель LOF
7. sensor_ml_part_3_OCSM - Модель OCSM

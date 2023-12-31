### Описание
Из банка стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.
Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

### Цель проекта
Построение модели для прогнозировния оттока клиентов банка. F1 модели >= 0.59

### Инструменты
* pandas
* numpy
* seaborn
* matplotlib
* sklearn

### Вывод:
* Подготовлены данные для дальнейшего исследования.
* Проведены масштибирование, борьба с дисбалансом.
* Исследованы модели Decision Tree Classifier, RandomForestClassifier и Logistic Regression.
* Проведена работа с дисбалансом техникой upsampling и downsampling. Лучший результат показала upsampling.
* Наилучшую эффективность показала модель RandomForestClassifier с гиперпараметрами n_estimators равным = 70 и max_depth = 14.
* На тестовой выборке модель достигла заданой метрики (F1 > 0.59) и показала адекватные результаты.
* Модель характеризуется достаточным показателем полноты равным 0.66 (min = 0, max = 1), поэтому она с достаточной вероятностью предскажет уход клиента из банка.
* Показатель точности равен 0.59 (min = 0, max = 1) — модель верно предсказывает больше половины ухода клиентов.
* Значение AUC-ROC = 0.85 говорит о том, что модель умеет предсказывать.

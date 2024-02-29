Решение задачи регрессии для набора данных Gold из PyCaret, содержащий 120 признаков, связанных с ценами на различные финансовые инструменты, включая некоторые товары и индексы.
В качестве целевой переменной используется Gold_T+22, т. е. строится модель регрессии, для предсказания цены Gold_T+22, учитывая показатели основных признаков.  
В исходном наборе данных между определенными признаками очень высокая корреляция, у четырех пар есть даже функциональная зависимость. Исходя из этого, были удалены столбцы, 
у которых коэффициент корреляции был по абсолютной величине выше 0,95. (Была проба удалить до 0.9, но это не привело к улучшению результата).  
Ниже в таблице результаты для исходного набора данных и сокращенного:  
|     | MAE | MSE| RMSE | R^2|Predic.R^2|
| ------------- |:------------------:| -----:|
| исходный dataset| 0.0146|0.0004|0.0204|0.7818|0.8779|
| сокращенный dataset| 0.0146|0.0004|0.0206|0.7795|0.8689|





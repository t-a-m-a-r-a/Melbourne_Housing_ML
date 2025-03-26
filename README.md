Ссылка на jupyter-notebook:
https://colab.research.google.com/drive/1XYFok7jEvlyCcky-F111yZ5P0KFnWXjQ?usp=sharing
# Цена дома в Мельбурне
Проект прогнозирования цены на недвижимость в Мельбурне
### Контекст
Задача состоит в определении ТОП самых важных параметров для прогнозирования цены дома, а также обучение модели её предсказания по характеристикам дома.

Источник данных: https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot?resource=download

### Стек проекта

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/-Seaborn-3776AB?style=flat-square&logo=seaborn&logoColor=white)
![Sklearn](https://img.shields.io/badge/-SkLearn-F89939?style=flat-square&logo=sklearn.&logoColor=white)

## Решение
### Шаг1

Провела EDA с помощью библиотеки pandas_profiling. По результатам анализа определила признаки к удалению во избежание переобучения модели, а также признаки с пропусками (для дальнейшего заполнения).

### Шаг2
Провела предобработку тренировочных и тестовых данных (заполнение пропусков, замена категориальных признаков).

### Шаг3
Обучила модели случайного леса и градиентного бустинга.  
По оценкам качества моделей градиентный бустинг дает результаты более близкие к реальным значениям.

## Результат

ТОП-3 самых важных признака для прогноза цены на дом - это район, количество комнат, удаленность от делового центра.
![Feature importance](https://github.com/user-attachments/assets/5e66288a-4572-4589-9e6a-9b1d53184c0e) 




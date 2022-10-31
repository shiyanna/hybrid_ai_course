# Извлечение онтологий из текста

## Предобработка текста
- сегментация
- регулярные выражения ([NLTK](https://www.nltk.org/))

## Векторизация текста
- удаление стоп-слов
- лемматизация ([SpaCy](https://spacy.io/models/ru))
- бинарный мешок слов ([sklearn](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html))

## Кластеризация токенов
- иерархическая кластеризация
  - агломеративная
  - дивизивная
- [кластеризация записей](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html) и [кластеризация признаков](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.FeatureAgglomeration.html)
- оптимизация
  - целевая функция: количество признаков
  - параметр: порог расстояния
  - метод локтя
- [визуализация дендрограммы](https://scikit-learn.org/stable/auto_examples/cluster/plot_agglomerative_dendrogram.html)
- функции объединения признаков

## Поиск ассоциативных правил
- ассоциативные правила
- [алгоритм "априори"](http://rasbt.github.io/mlxtend/api_subpackages/mlxtend.frequent_patterns/#association_rules)
- метрики
  - суппорт
  - конфиденс
  - лифт
- импликации

## Создание онтологии
- классы и экземпляры
- создание экземпляров на основе предложений
- создание классов на основе токенов
- связь между предложениями и токенами
- создание классов на основе кластеров
- связь между кластерами и токенами
- построение иерархии кластеров
- логическая интерпретируемая кластеризация предложений с помощью ризонера

---
[Запись лекции](https://youtu.be/klX6o2_SoJ8)

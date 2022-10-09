# Обучение деревьев решений без учителя и их конвертация в онтологию

## Предобработка данных
- [стандартизация](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)
- визуализация данных с помощью [метода главных компонент](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)

## Обучение деревьев решений без учителя
- генерация уникальных лейблов
- поиск оптимума гиперпараметра min impurity decrease последовательным перебором
  - обучение дерева
  - получение [silhouette score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.silhouette_score.html)
- построение графика min impurity decrease/silhouette score
- выбор оптимума [методом локтя](https://en.wikipedia.org/wiki/Elbow_method_(clustering)) (расчет silhouette score gain)
- визуализация дерева

## Дескрипционные логики
- [дескрипционная логика](https://en.wikipedia.org/wiki/Description_logic#The_description_logic_ALC)
  - выразимость/вычислимость
  - синтаксис
  - семантика
- [табличный алгоритм](https://en.wikipedia.org/wiki/Method_of_analytic_tableaux)

## Построение иерархии OWL классов
- извлечение данных из обученного дерева, для каждого узла указывается
  - идентификатор
  - идентификатор родителя
  - признак
  - граница
  - тип сравнения
- библиотека [owlready2](https://owlready2.readthedocs.io/en/latest/)
- создание онтологии
- создание DataProperty на основе признаков набора данных
- создание классов
  - нахождение класса родителя по идентификатору
  - создание класса с указанием лейбла и суперкласса
  - ограничение класса с помощью свойства EquivalentTo, признака, границы и типа сравнения
 
 ## Создание экземпляров и логическая классификация
 - создание экземпляра без класса
 - указание значений DataProperty на основе данных
 - запуск ризонера

---
[Запись лекции](https://youtu.be/xEf8GsOxvw8)

---
[Лабораторная работа](https://github.com/ldrbmrtv/hybrid_ai_course/blob/main/udt2owl/task.md)

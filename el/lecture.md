# Федеративное обучение и эпистемическая логика

## [Федеративное обучение](https://en.wikipedia.org/wiki/Federated_learning)

## Классификаторы
- [наивный байесвоский классификатор](https://scikit-learn.org/stable/modules/naive_bayes.html)
- [К ближайших соседей](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html#sklearn.neighbors.KNeighborsClassifier)
- [метод опорных векторов](https://scikit-learn.org/stable/modules/svm.html#svm-classification)

## [Эпистемическая логика](https://en.wikipedia.org/wiki/Epistemic_modal_logic)
- [модальные логики](https://en.wikipedia.org/wiki/Modal_logic)
- cинтаксис
- cемантика
- логический вывод
- [доксастическая логика (логика мнений)](https://en.wikipedia.org/wiki/Doxastic_logic)

## Имплементация эпистемической логики в онтологии
- возможные миры -> индивиды
- отношение эпистемической неразличимости -> рефлексивное, симметричное, транзитивное ObjectProperty r1
- отношение доксастической неразличимости -> симметричное, транзитивное ObjectProperty r2
- высказывание -> класс A
- модальный оператор Ka -> класс KnowA equivalentTo r1 only A
- модальный оператор Ba -> класс BelieveA equivalentTo r2 only A

## Эпистемико-онтологическая модель федеративного обучения
- онтология как эпистемический агент
- генерация классов KnowL и BelieveL для каждого лейбла L
- генерация индивида для каждого предикта каждого классификатора
- установление неразличимости для индивидов, относящихся к одной записи набора данных
- логический вывод производных отношений неразличимости
- замыкание индивидов
- логическая классификация индивидов

---
[Запись лекции](https://youtu.be/zARpf-_PDSo)

---
[Лабораторная работа](https://github.com/ldrbmrtv/hybrid_ai_course/blob/main/el/task.md)

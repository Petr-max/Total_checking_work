# Итоговая проверочная работа.

Данная работа необходима для проверки ваших знаний и навыков по итогу 
прохождения первого блока обучения на программе разработчик. 
Мы должны убедиться что базовое знакомство с it прошло успешно.
Задача алгоритмически не самая сложная, однако для полценного 
выполнения проверочной работы необходимо:

1. Создать репозиторий на GitHub

2. Нарисовать блок-схему алгоритма (можно обойтись блок-схемой основной содержательной части, 

если вы выделяете ее в отдельный метод)

3. Снабдить репозиторий оформленным текстовым описанием решения (файл README.md)

4. Написать программу, решающую поставленную задачу

5. Использовать контроль версий в работе над этим небольшим проектом (не должно быть так 

что все залито одним коммитом, как минимум этапы 2, 3 и 4 должны быть расположены в разных коммитах)

## Задача: 

Написать программу, которая из имеющегося массива строк формирует массив из строк, 
длина которых меньше либо равна 3 символа.
Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. 
При решении не рекомендуется пользоваться коллекциями, 
лучше обойтись исключительно массивами.

## Примеры:

**['hello", "2", "world", ":-)"] -> ["2", "-)"]**

**["1234", "1567", "-2", "computer science"] -> ["-2"]**

**["Russia", "Denmark", "Kazan"] -> []**

## Решение:

1. При запуске программы у пользователя запрашивается длина массива.
2. С помощью цикла пользователь заполняет массив значениями массива.
3. В методе `SizeModifiedArray` происходит следующее:
- Создается переменная `count`, в которой будет содержаться длина для нового массива.
- С помощью цикла `for`, который работает пока `i` меньше длины массива, проверяется условие: 
- если элемент массива меньше 3, то к переменной `count` плюсуется единица.
- После завершения всех итераций происходит возврат `count`.
4. В методе `ModifiedArray` происходит следующее:
- Создаются новый массив `newArray`, переменные `i` и `j`.
- В цикле `while`, который работает пока `j` меньше длины массива, проверяется условие: 
- если элемент массива меньше 3, то элементу `i` нового массива присваивается 
- значение элемента `j` исходного массива.
- После завершения всех итераций происходит возврат нового массива.
5. С помощью метода `PrintArray` выводится исходный массив.
6. С помощью метода `PrintArray` выводится новый массив.

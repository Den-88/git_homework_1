## СТРОКА ДЛЯ НАГЛЯДНОСТИ! Добавил при ручном разрешении конфликта.
# Задание 1. Создайте программу на Python или Java, которая принимает два списка чисел и выполняет следующие действия:

a. Рассчитывает среднее значение каждого списка.

b. Сравнивает эти средние значения и выводит соответствующее сообщение:
- "Первый список имеет большее среднее значение", если среднее значение первого списка больше.
- "Второй список имеет большее среднее значение", если среднее значение второго списка больше.
- "Средние значения равны", если средние значения списков равны.
 
# Решение:

- [Код программы (ListComparator.java)](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/src/ListComparator.java)
- [Код тестов (ComparatorTests.java)](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/test/ComparatorTests.java)
- [Скриншот проверки кода с помощью Checkstyle](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/checkstyle_screenshot.png)
![Скриншот проверки кода с помощью Checkstyle](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/checkstyle_screenshot.png)
- [Скриншот отчета о покрытии тестами](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/tests_caverage_screenshot.png)
![Скриншот отчета о покрытии тестами](https://github.com/Den-88/testing/blob/homework_6/HomeWork6/tests_caverage_screenshot.png)
- Объяснение того, какие сценарии покрыты тестами и почему вы выбрали именно эти сценарии:
1. `testCalculateAverage`: Этот тест проверяет правильность вычисления среднего значения списка. В качестве входных данных используется список чисел `[8, 5, 2]`, и ожидается, что среднее значение будет равно `5.0`. Этот сценарий выбран для проверки корректности реализации метода `calculateAverage`.

2. `testCalculateEmptyList`: Этот тест проверяет правильность вычисления среднего значения пустого списка. В качестве входных данных используется пустой список, и ожидается, что среднее значение будет равно `0`. Этот сценарий выбран для проверки корректной обработки пустого списка в методе `calculateAverage`.

3. `testCompareFirstListLarger`: Этот тест проверяет сравнение списков, когда среднее значение первого списка больше среднего значения второго списка. В качестве входных данных используются списки `[9, 7, 3]` и `[3, 5, 1]`, и ожидается, что результат сравнения будет строкой `"Первый список имеет большее среднее значение"`. Этот сценарий выбран для проверки правильности работы метода `compareLists` в случае, когда первый список имеет большее среднее значение.

4. `testCompareSecondListLarger`: Этот тест проверяет сравнение списков, когда среднее значение второго списка больше среднего значения первого списка. В качестве входных данных используются списки `[1, 2, 3]` и `[4, 5, 6]`, и ожидается, что результат сравнения будет строкой `"Второй список имеет большее среднее значение"`. Этот сценарий выбран для проверки правильности работы метода `compareLists` в случае, когда второй список имеет большее среднее значение.

5. `testCompareListsEqual`: Этот тест проверяет сравнение списков, когда средние значения обоих списков равны. В качестве входных данных используются списки `[1, 2, 3]` и `[4, 0, 2]`, и ожидается, что результат сравнения будет строкой `"Средние значения равны"`. Этот сценарий выбран для проверки правильности работы метода `compareLists` в случае, когда средние значения обоих списков равны.

   Выбор этих сценариев обусловлен необходимостью проверки различных случаев использования программы, чтобы убедиться в правильности работы методов `calculateAverage` и `compareLists` в различных ситуациях. Тесты позволяют проверить основные функциональности программы и обнаружить возможные ошибки или неправильное поведение.



*Иван Солнцев. 01.12.2022 GeekBrains. Разработчик.*

# Итоговая работа 1 четверти обучения

## Задача 1. Создать репозиторий на GitHub

>Путь к репозиторию: https://github.com/SunRay-35/Sun_Q1_Final.git

## Задача 2. Нарисовать блок-схему алгоритма

Блок схема представлена в корне проекта в файлaх:
> diagram.drawio

> diagram.png
![Диаграмма в формате PNG](/diagram.png)

## Задача 3. Снабдить репозиторий оформленным текстовым описанием решения

>Файл: README.md

## Задача 4. Написать программу, решающую поставленную задачу.

>Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Решение задачи основывается на методе **Array.Resize()**. Так как в C# размерность массивов фиксируется на момент их объявления, то необходимо использовать промежуточный массив для изменения размерности текущего массива.

Можно было бы реализовать такой метод пользовательским кодом, но **Array.Resize()** выполняет именно эту функцию. На вход подаются два параметра(**ref array**, **length**), где **array** - это имя текущего массива, у которого необходимо изменить размер, а **length** - это новая длина массива. Метод создаст временный массив с необходимой длиной, сделает копию значений элементов исходного массива и присвоит текущему массиву содержимое нового временного.

Остальное решение - это стандартный метод перебора массива в цикле **for** и проверка на соответствие условиям задачи через оператор **if**.

> Основные методы

1. **Main()** - основное тело программы, не возвращает результат.
2. **PrintArray()** - метод получает на вход строковый одномернный массив **array** и выводит его в консоль, не возращает результат. В качестве дополнительной переменной на вход подается строка **message**, которая является сопроводительным текстом к самому массиву и выводится перед ним.
3. **ParseArray()** - метод получает на вход строковый одномернный массив **arraySource** и преобразует его во временный массив **arrayTemp** с учетом поставленной задачи. Возвращает новый строковый массив **arrayTemp**.

## Задача 5. Использовать контроль версий в работе над этим проектом.

1. Создан репозиторий и добавлен файл .gitignore для C# проектов.
2. Созданы файл README.md и проект диаграммы, на базе которой будет написан код.
3. Создана типовая структура проекта C# - консольное приложение.
4. Реализована программа, которая решает поставленную задачу.
5. Диаграмма скорректирована с учетом реализованной программы.
6. Внесены правки и созданы необходимые файлы для завершения проекта.

# Итоговая работа завершена

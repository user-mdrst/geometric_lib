## Описание
В данной лабораторной работе изучаются основы модульного тестирования в Python с использованием библиотеки unittest.
Тестируются функции для расчёта площади и периметра (или аналогичных характеристик) различных геометрических фигур: прямоугольника, квадрата, треугольника и круга.

## Структура проекта
- lab4/
  - rectangle.py          (Функции area(a, b), perimeter(a, b))
  - circle.py             (Функции area(r), perimeter(r))
  - square.py             (Функции area(a), perimeter(a))
  - triangle.py           (Функции area(a, h), perimeter(a, b, c))
  - rectangle_test.py     (Unit-тесты для rectangle.py)
  - circle_test.py        (Unit-тесты для circle.py)
  - square_test.py        (Unit-тесты для square.py)
  - triangle_test.py      (Unit-тесты для triangle.py)
  - Lab4_UnitTests_Report.pdf  (Отчет по лабораторной работе)

## Установка
1. Клонируйте репозиторий:
   git clone <URL вашего репозитория>
   cd Lab4_UnitTests
2. Убедитесь, что установлен Python 3.8+
3. Библиотека unittest входит в стандартную поставку Python, установка дополнительных пакетов не требуется

## Запуск тестов

Через командную строку:
- python -m unittest rectangle_test.py
- python -m unittest circle_test.py
- python -m unittest square_test.py
- python -m unittest triangle_test.py

Или запустить все тесты сразу:
- python -m unittest discover

Через PyCharm Unit Test Runner:
- Правый клик по файлу теста → Run 'Python tests in <file>'
- Или нажать зелёный треугольник слева от имени класса тестов

Вывод тестов при успешном выполнении:
Ran X tests in Y seconds
OK

## Содержание тестов
Каждый тест проверяет функции:
- area() — площадь фигуры
- perimeter() — периметр фигуры

Покрыты следующие случаи:
- нормальные значения (положительные числа)
- граничные значения (0)
- негативные значения (отрицательные числа)
- для круга — проверка с использованием math.pi и assertAlmostEqual

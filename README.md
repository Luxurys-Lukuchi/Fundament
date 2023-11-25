# Класс Foundation

Класс Foundation представляет фундамент из бетона. Он имеет следующие атрибуты и методы:

## Атрибуты

- `length`: длина фундамента в метрах
- `width`: ширина фундамента в метрах
- `height`: высота фундамента в метрах
- `density`: плотность материала фундамента в килограммах на кубический метр
- `concreteGrade`: марка бетона, которая может быть одной из следующих: `M100`, `M200`, `M300`, `M400`, `M500`

## Методы

- `Foundation()`: конструктор по умолчанию, который инициализирует атрибуты нулевыми значениями и маркой бетона `M100`
- `setLength(double len)`: метод для установки значения длины фундамента с проверкой на положительность
- `getLength()`: метод для получения значения длины фундамента
- `setWidth(double wid)`: метод для установки значения ширины фундамента с проверкой на положительность
- `getWidth()`: метод для получения значения ширины фундамента
- `setHeight(double hei)`: метод для установки значения высоты фундамента с проверкой на положительность
- `getHeight()`: метод для получения значения высоты фундамента
- `setConcreteGrade(ConcreteGrade grade)`: метод для установки марки бетона с соответствующим расчетом плотности
- `getConcreteGrade()`: метод для получения марки бетона
- `calculateArea()`: метод для расчета площади поверхности фундамента
- `calculateVolume()`: метод для расчета объема фундамента
- `calculateMass()`: метод для расчета массы фундамента
- `calculatePressureForce()`: метод для расчета силы давления фундамента на землю
- `calculateCost()`: метод для расчета стоимости фундамента
- `testFoundation()`: метод для тестирования работы класса с помощью утверждений
- - `testFoundation()`: метод для тестирования работы класса с помощью утверждений
- `operator<(const Foundation& other)`: перегруженный оператор сравнения для сравнения фундаментов по площади
- `outputInformationConsole()`: метод для вывода информации о фундаменте в консоль
- `concreteGradeToString()`: метод для преобразования марки бетона в строку
- `saveToFile(const std::string& filename)`: метод для сохранения информации о фундаменте в текстовый и бинарный файлы
- `loadFromFile(const std::string& filename)`: метод для загрузки информации о фундаменте из бинарного файла
- - `deleteDynamicArray(Foundation** array, int size)`: статический метод для удаления динамического массива фундаментов
##  функции main
- `main()`: функция main, которая демонстрирует работу класса Foundation с помощью ввода и вывода данных, сохранения и загрузки информации из файлов и поиска фундамента с минимальной площадью
-  функция main продолжает работу с динамическим массивом фундаментов, который был создан и инициализирован в предыдущем разделе
- Для каждого фундамента в массиве, выполняются следующие действия:
  - Ввод марки бетона из списка возможных вариантов
  - Установка марки бетона и соответствующей плотности для фундамента
  - Сохранение информации о фундаменте в текстовый и бинарный файлы с помощью метода `saveToFile`
  - Расчет стоимости фундамента с помощью метода `calculateCost` и вывод на экран
  - Поиск фундамента с минимальной площадью с помощью перегруженного оператора `<` и обновление переменных `minArea` и `indexMinArea`
- После цикла, выводится информация о фундаменте с минимальной площадью с помощью метода `outputInformationConsole`, если такой фундамент найден
- Затем, освобождается память, выделенная для динамического массива фундаментов, с помощью статического метода `deleteDynamicArray`
- Функция main возвращает 0 и завершает работу программы

## Читать
- [C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 3.* Creating Types in C#
   - *Chapter 7:* Collections. The Array Class
- [C# 5.0 Unleashed. Bart De Smet. Sams Publishing. 2013.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 4.* Language Essentials. Arrays
   - *Chapter 9.* Introducing Types
- [Коллекции в .NET Framework Class Library. Массивы](http://rsdn.ru/article/dotnet/collections.xml#E2GAC)
- [C#: Внутреннее строение инициализаторов массивов](http://habrahabr.ru/post/247047/)

## Материалы (презентация)
- [Basic Coding in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M4.%20Methods%20in%20details)
- [Creating types in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M3.%20Creating%20types%20in%20C%23)
- [LINQPad примеры](https://drive.google.com/drive/u/0/folders/1_uY1tmKK3WlFkB5PsyqjJsWP6-DYhvoY)

## Задачи (deadline - 18.00 25.03.2018)
- (**deadline - 18.00 24.03.2018**) Реализовать метод расширения для получения строкового двоичного представления вещественного числа двойной точности в формате IEEE 754 (**при реализации готовые  классы-конверторы не использовать!**). Разработать модульные тесты. (NUnit фреймворк)
  - [TestCase(-255.255, ExpectedResult = "1100000001101111111010000010100011110101110000101000111101011100")]
  - [TestCase(255.255, ExpectedResult = "0100000001101111111010000010100011110101110000101000111101011100")]
  - [TestCase(4294967295.0, ExpectedResult = "0100000111101111111111111111111111111111111000000000000000000000")]
  - [TestCase(double.MinValue, ExpectedResult = "1111111111101111111111111111111111111111111111111111111111111111")]
  - [TestCase(double.MaxValue, ExpectedResult = "0111111111101111111111111111111111111111111111111111111111111111")]
  - [TestCase(double.Epsilon, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000001")]
  - [TestCase(double.NaN, ExpectedResult = "1111111111111000000000000000000000000000000000000000000000000000")]
  - [TestCase(double.NegativeInfinity, ExpectedResult = "1111111111110000000000000000000000000000000000000000000000000000")]
  - [TestCase(double.PositiveInfinity, ExpectedResult = "0111111111110000000000000000000000000000000000000000000000000000")]
  - [TestCase(-0.0, ExpectedResult = "1000000000000000000000000000000000000000000000000000000000000000")]
  - [TestCase(0.0, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000000")]   
и т.д.  

![К решению](https://github.com/AnzhelikaKravchuk/Training.-Spring-2018/blob/master/Pictures/ToIEEE754.png) 

- (**deadline - 18.00 24.03.2018**) Реализовать метод расширения получения из строкового представления целого положительного четырехбайтового числа, записанного в p-ичной системе счисления (2<=p<=16), его десятичного значения (**при реализации готовые классы-конверторы не использовать!**). Разработать модульные тесты. (NUnit фреймворк). Примерные тесткейсы.
    - "0110111101100001100001010111111" для основания 2 -> 934331071
    - "01101111011001100001010111111" для основания 2 -> 233620159
    - "11101101111011001100001010" для основания 2 -> 62370570
    - "1AeF101" для основания 2 -> ArgumentException
    - "11111111111111111111111111111111" для основания 2 -> OverflowException
    - "1AeF101" для основания 16 -> 28242177
    - "1ACB67" для основания 16 -> 1756007
    - "SA123" для основания 2 -> ArgumentException
    - "764241" для основания 8 -> 256161   
    - "764241" для основания 20 -> ArgumentException  
    - "10" для основания 5 -> 5   
  и т.д.   
  
![К решению](https://github.com/AnzhelikaKravchuk/Training.-Spring-2018/blob/master/Pictures/ToConverter.png) 

- Разработать неизменяемый класс Polynomial (полином) для работы с многочленами степени  от одной переменной вещественного типа (в качестве внутренней структуры для хранения коэффициентов использовать sz-массив). Для разработанного класса переопределить виртуальные методы класса Object; перегрузить операции, допустимые для работы с многочленами (исключая деление многочлена на многочлен), включая "==" и "!=". Разработать unit-тесты (NUnit фреймворк).
- Реализовать метод "пузырьковой" сортировки непрямоугольного ("jagged" array) целочисленного массива (не использовать методы класса System.Array!) таким образом, чтобы была возможность упорядочить строки матрицы:
   - в порядке возрастания(убывания) сумм элементов строк матрицы;
   - в порядке возрастания(убывания) максимальных элементов строк матрицы;
   - в порядке возрастания(убывания) минимальных элементов строк матрицы.

   Разработать unit-тесты (NUnit фреймворк).

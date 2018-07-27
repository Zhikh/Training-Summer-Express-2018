## Читать (Обязательно!)
- Programming C# 5.0. Ian Griffiths. O'Reilly Media. 2012. Chapter 5. Collections.
- C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015. Chapter 7. Collections.
  - *Основное внимание уделить следующим обобщенным строго типизированным коллекциям - List, Queue, Stack, Sets, Dictionaries.*
  - *Обязательно ознакомиться с **Plugging in Equality and Order** (C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015. Chapter 7. Collections)*
  - [Откуда растут руки у GetHashCode в .NET](https://habrahabr.ru/post/188038/)
  - [Правила и рекомендации по переопределению GetHashCode](https://blogs.msdn.microsoft.com/ruericlippert/2011/03/20/943/)
- [LINQ](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M11.%20Introduction%20to%20Language%20Integrated%20Query%20(LINQ))

## Материалы (презентация)
- [Generics and Collections](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M10.%20Generics%20and%20Collections)
- [LINQ](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M11.%20Introduction%20to%20Language%20Integrated%20Query%20(LINQ))
- [LINQPad Generics and Collections](https://drive.google.com/drive/u/0/folders/1Jn7byrj6lMiV-tKuMdA-_p3JoiEgWf9N)

## Задачи 
1. **(deadline - 26.07.2018, 24.00)** Разработать обобщенный класс-коллекцию BinarySearchTree (бинарное дерево поиска). Предусмотреть возможности использования подключаемого интерфейса для реализации отношения порядка. Реализовать три способа обхода дерева: прямой (preorder), поперечный (inorder), обратный (postorder): для реализации использовать блок-итератор (yield). Протестировать разработанный класс, используя следующие типы:
  - System.Int32 (использовать сравнение по умолчанию и подключаемый компаратор); 
  - System.String (использовать сравнение по умолчанию и подключаемый компаратор); 
  - пользовательский класс Book, для объектов которого реализовано отношения порядка (использовать сравнение по умолчанию и подключаемый компаратор); 
  - пользовательскую структуру Point, для объектов которого не реализовано отношения порядка (использовать подключаемый компаратор).
2. **(deadline - 27.07.2018, 24.00)** Предложить различные способы (2-3 способа) описания класса TrafficLight (Светофор) для системы управления различными светофорами, соответствующий принципам ООП.

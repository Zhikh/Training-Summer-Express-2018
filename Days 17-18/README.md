## Читать
- [Object Oriented Design Principles](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M16.%20Object%20Oriented%20Design%20Principles)
- [Примеры использования Moq](https://habr.com/post/150859/)
- [The Art of Unit Testing: with examples in C# Second Edition Edition. Roy Osherove.  Manning Publications Co. 2013.](https://www.manning.com/books/the-art-of-unit-testing-second-edition)
   - *Chapter 3.* [Using stubs to break dependencies](https://livebook.manning.com/#!/book/the-art-of-unit-testing-second-edition/chapter-3/1)
   - *Chapter 4.* [Interaction testing using mock objects](https://livebook.manning.com/#!/book/the-art-of-unit-testing-second-edition/chapter-4/1)


## Материалы (презентация)
- [Принципы проектирования](https://drive.google.com/drive/u/0/folders/1ycAPdDl9y3fYsQrUCAP58f5h7fWpOeRV)
- [LSP](https://drive.google.com/drive/u/0/folders/1ycAPdDl9y3fYsQrUCAP58f5h7fWpOeRV)
- [LINQPad](https://drive.google.com/drive/u/0/folders/1qWNm-Ruph09xPQ3A0WQx9s3YKDYyhv9b)
- [Примеры использования Moq](https://drive.google.com/drive/u/0/folders/1ycAPdDl9y3fYsQrUCAP58f5h7fWpOeRV)

## Задачи (deadline)
1. Разработать систему типов для описания работы с банковским счетом. Состояние счета определяется его номером, данными о владельце счета (имя, фамилия, e-mail), суммой на счете и некоторыми бонусными баллами, которые увеличиваются/уменьшаются каждый раз при пополнении счета/списании со счета на величины различные для пополнения и списания и рассчитываемые в зависимости от некоторых значений величин «стоимости» баланса и «стоимости» пополнения. Величины «стоимости» баланса и «стоимости» пополнения являются целочисленными значениями и зависят от типа счета, который может быть, например,  Base, Gold, Platinum. Для работы со счетом реализовать следующие возможности: 
   - выполнить пополнение на счет;
   - выполнить списание со счета; 
   - создать новый счет; 
   - закрыть счет.  
    
    Для хранения информации о счетах использовать fake-имплементацию репозитория (хранилища) в виде класса-обертки для коллекции List<Account>.
 
    Работу классов продемонстрировать на примере консольного приложения. 

    При проектировании типов учитывать следующие возможности расширения/изменения функциональности
      - добавление новых видов счетов;
      - изменение/добавление источников хранения информации о счетах;
      - изменение логики расчета бонусных баллов;
      - изменении логики генерации номера счета.
  
    Для организации классов и интерфейсов использовать “The Stairway pattern” (“заготовка” в архиве [AccountSystemDemo.7z](https://github.com/AnzhelikaKravchuk/Training.-Spring-2018/blob/master/Day%2017/AccountSystemDemo.7z)). 
  
    Для разрешения зависимостей использовать Ninject- фреймворк.

    Протестировать слой Bll (NUnit и Moq фреймворки).

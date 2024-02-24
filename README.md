Я створив HTML документ, що створює простий веб-інтерфейс, де студент може запустити процес генерації випадкової послідовності, її скремблування та подальшого декремблування за допомогою кнопки. 

Крок 1: Створення функцій скремблування та декремблування
Скремблер використовує адитивний метод, де кожен біт вхідної послідовності складається за модулем 2 з відповідним бітом псевдовипадкової послідовності, що генерується зсувним регістром. Декремблер виконує зворотну операцію.

Крок 2: Генерація випадкової послідовності
Функція генерує випадкову послідовність 0 і 1 завдовжки K=1000.

Крок 3: Тестування функцій
Ми скремблюємо випадкову послідовність, а потім декремблюємо отриману послідовність, щоб перевірити, чи отримаємо ми на виході початкову послідовність.

Крок 4: Порівняння послідовностей
Поелементно порівняємо вихідну та декрембліровану послідовності, щоб переконатися у правильності роботи алгоритмів.

Дані за варінтом:
Тип кремблера / дескремблера - Адитивний  
Н - 10 
Зсувний регістр - 10010001001 

Важливо відмітити, що функція написана на голому ЖС, без використання сторонніх бібіотек та готови рішень.

Кнопка button, при натисканні на яку викликається функція generateAndDisplaySequences(), що генерує та відображає послідовності.
Блок для результатів div id="results", де будуть відображені результати генерації, скремблювання та дескремблювання послідовностей.
В документі також міститься скрипт, що включає в себе кілька функцій:

generateRandomSequence(length) - генерує випадкову послідовність заданої довжини.
scramble(inputSequence, shiftRegister) - скремблює вхідну послідовність за допомогою зсувного регістру.
descramble(inputSequence, shiftRegister) - дескремблює вхідну послідовність, також використовуючи зсувний регістр.
generateAndDisplaySequences() - інтегрує вищезазначені функції для генерації оригінальної послідовності, її скремблювання, дескремблювання та відображення результатів на сторінці.

Короткі висновки:
Цей код ініціалізує зсувний регістр заданим значенням і використовує його для адитивного скремблування та декремблування послідовності. Результати показуються у вигляді тексту під кнопкою. 
Результати (перші 10 бітів кожної послідовності) відображаються на сторінці, що дозволяє легко порівняти оригінальну, скрембльовану та декрембльовану послідовності.
JavaScript код забезпечує однаковий початковий стан зсувного регістру для процесів скремблування та декремблування. Це гарантує, що декрембльована послідовність точно відповідає оригінальній.( перевірка тру або фолс)
Перевірити можна вручні викрпистовуючи консоль розробника (Ф12)

# timetable_lab

## First part - genetic algorithm

Перша частина - генетичний алгоритм
Використовуйте генетичний алгоритм і python для ефективного розподілу вчителів по групах.

Щоб запустити genetic_alg.py потрібно:

встановити групи студентів у верхній частині основного файлу (або залишити без змін)
встановити вчителів (або залишити без змін)
встановити розмір популяції та кількість ітерацій (або залишити без змін)
запустити genetic_alg.py
перевірте результати: перший рядок — максимально можливий бал, потім ви можете побачити прогрес локального максимуму через ітерації. Тоді ви побачите найкращий знайдений розклад. У нижній частині результату ви можете порівняти показники випадкової популяції та популяції після генетичного алгоритму.
Приклад останньої вихідної частини:

```
-----genetic algorithm-----
@@@@ average score: 46.03125
@@@@ best score: 49
-----simple population-----
@@@@ average score: 38.4296875
@@@@ best score: 47
```

Як бачимо, середній бал популяції значно підвищується.

## Second part - CSP algorithm

Потім ми вирішуємо проблему задоволення обмежень, щоб призначити вчителям і групам правильні години та дні.

Код для алгоритму CSP зберігається у файлі CSP.py.

Щоб отримати остаточний розклад - запустіть файл main.py.

Приклад результату:

```
Monday
1: 1A english (john) 1B history (alice) 1C english (bob) 1D math (mike) 
2: 1A english (john) 1B history (alice) 1C english (bob) 1D math (mike) 
3: 1A history (bob) 1B english (john) 1C math (sarah) 1D science (victor) 
4: 1A history (bob) 1B english (john) 1C math (sarah) 1D science (victor) 

Tuesday
1: 1A history (bob) 1B english (john) 1C science (sam) 1D science (victor) 
2: 1A history (bob) 1B english (john) 1C science (sam) 1D science (victor) 
3: 1A history (bob) 1B literature (james) 1C science (sam) 1D science (victor) 
4: 1A math (mike) 1B literature (james) 1C history, arts (alice) 1D literature, arts (jane) 

Wednesday
1: 1A math (mike) 1B literature (james) 1C history, arts (alice) 
2: 1A literature (jane) 1C literature (james) 
3: 1A literature (jane) 1C literature (james) 
4: 1A literature (jane) 

Thursday
1: 1A literature (jane) 
2: 1A literature (jane) 
3: 1A literature (jane) 
4: 1A arts (alice) 1B arts (jane) 

Friday
1: 1A arts (alice) 1B arts (jane) 
2: 1A arts (alice) 1B arts (jane) 
```

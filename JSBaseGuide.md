**Базова термінологія**
=

Інструкція 
a = b * 2;
a i b - змінні
"* / + -" - оператори

Вираз

![5e8aade5-549a-44d2-ad5a-359efb201dd3m01-b01-s04](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/87d66b93-756e-481e-a1e7-a6d91167f7e9)

Літерал
// Числовий літерал
10

// Рядковий літерал
"JavaScript is awesome!"

**Підключення скрипта**
=

// Вбудований скрипт

<head>
    <title>My HTML-page</title>
    <script>
        <!--Твій JavaScript-код тут-->
        console.log("Hello, world");
    </script>
</head>

// Зовнішній скрипт

<head>
    <title>My HTML-page</title>
    <script src="my-script.js" defer></script>
</head>

Але краще всього скрипт завжди додавати в кінець тегу <body>, або ж не забувати прописувати defer у тегах!

**Суворий режим**
=

'use strict';

// Код у суворому режимі

-!- Рекомендується завжди використовувати суворий режим у своїх проєктах, щоб уникнути непередбачуваних ситуацій і проблем у коді.

**Виведення даних**
=

<img width="733" alt="0656e9d3-94d1-4cba-aba5-8ad39abb85dbScreenshot 2023-07-04 at 16 51 35" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a2a15a15-3364-46da-9ba4-0d8e5b3d40d6">

Наступні комбінації клавіш відкривають інструменти розробника на вкладці Console:
Windows і Linux — Ctrl + Shift + J;
MacOS — Command + Option + J .

Щоб вивести дані в консоль розробника використовується метод console.log()

console.log("JavaScript is awesome!");
console.log(10);

<img width="662" alt="2e0efa32-9ccb-4dcc-80b3-46d0ea254b72Screenshot 2023-07-04 at 16 58 55" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/726b585b-eba3-4469-b0bd-3a8c690848e1">

**Оголошення змінних**
=

let age = 20 
const username = "Mango"

Ключове слово (let / const) => назва змнної (age, username (може буьт будь-яка)) => змінна (20, "Mango")

**Перевизначення змінних**
=

<img width="424" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f26196cb-861c-437d-9d2f-9ec2581cde0f">

Змінну let можна змінити, змінну const - ні!

<img width="636" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e0fb1df1-06c7-4c97-8a7b-a79ac873af07">

**Найменування**
=

<img width="279" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f8e65e21-ad2e-434a-80d9-9f41907e303f">

Варто пам'ятати, що існують зарезервовані **ключові слова**

![9f4e2b98-8e94-46de-a640-f03c05f39327m01-b02-s04](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/2280e368-0b19-465b-84cd-bc91c168fbdb)

**Типи даних**
=

**Number**

const age = 20;
const salary = 3710.84;

**String**

const username = 'Mango995';
const description = "JavaScript is awesome!";

**Boolean**

const isModalOpen = true;
const isLoggedIn = false;

**Спеціальні значення**
=

let value = null;
console.log(value); // null

let value;
console.log(value); // undefined

Хоча обидва значення null і undefined позначають відсутність значення, вони мають трохи різні семантики використання.
 — null використовується для явної вказівки порожнього значення (точно відомо, що значення немає).
 — undefined вказує на невизначеність значення змінної.

**Оператор typeof**
=

typeof operand - Замість operand ти вказуєш змінну, літерал або вираз, тип якого ти хочеш визначити. Результатом оператора typeof буде рядок, який вказує тип даних.

**Арифметичні операції**
=

<img width="340" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c835dee6-c5f0-4490-90a6-f393c18ba1c5">

Оператор (+) використовується для складання двох чисел.
Оператор (-) використовується для віднімання одного числа від іншого.
Оператор (*) використовується для множення двох чисел.
Оператор (/) використовується для ділення одного числа на інше.
Оператор (%) повертає остачу від ділення одного числа на інше.
Оператор (**) використовується для піднесення числа до степеня.

**Комбіновані оператори**
=

Додавання: +=. Приклад: x += y еквівалентно x = x + y

Віднімання: -=. Приклад: x -= y еквівалентно x = x - y

Множення: *=. Приклад: x *= y еквівалентно x = x * y

Ділення: /=. Приклад: x /= y еквівалентно x = x / y

Остача від ділення: %=. Приклад: x %= y еквівалентно x = x % y

**Конкатенація рядків**
=

Якщо застосувати оператор + до рядка та будь-якого іншого типу даних, результатом буде новий рядок, що містить об'єднання вихідних значень.

const message = "Mango " + "is" + " happy";
console.log(message); // "Mango is happy"

console.log("Mango" + 55); // "Mango55"
console.log("Mango" + true); // "Mangotrue"

console.log(1 + "2"); // "12"
console.log(1 + "2" + 4); // "124"
console.log(1 + 2 + "4"); // "34"

**Перетворення типів: рядки**
=

**Явне перетворення типів**

console.log(String(5)); // "5"
console.log(String(true)); // "true"
console.log(String(false)); // "false"
console.log(String(null)); // "null"
console.log(String(undefined)); // "undefined"

**Неявне перетворення типів**

console.log("5" + 3); // "53"
console.log("5" + true); // "5true"
console.log("5" + false); // "5false"
console.log("5" + null); // "5null"
console.log("5" + undefined); // "5undefined"

**Шаблонні рядки**
=

Шаблонні рядки огортаються зворотними лапками (англ. backticks) (``)

Увага! 
Код не працюватиме, якщо огорнути шаблонні рядки звичайними одинарними або подвійними лапками.

**Довжина рядка**
=

Для доступу до властивості (property) сутності (objectName) використовується синтаксис із крапкою:
сутність.властивість

У програмуванні, наприклад, рядок має властивість length, яка повертає довжину рядка.

const productName = "Repair droid";

// Якщо у змінній зберігається рядок
console.log(productName.length); // 12

// Якщо рядковий літерал
console.log("Repair droid".length); // 12

**Індексація рядків**
=

![72eb24ab-b422-4ed8-afb7-1c03955121d7m01-b03-s06](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/bc1dd07b-5212-4269-9b92-ec2c1091226b)

**Оператори порівняння**
=

Оператор > (більше) — повертає true, якщо лівий операнд більше правого. В іншому разі повертає false .

Оператор < (менше) — повертає true, якщо лівий операнд менше правого. В іншому разі повертає false .

Оператор >= (більше або дорівнює) — повертає true, якщо лівий операнд більше або дорівнює правому. Якщо навпаки, повертає false .

Оператор <= (менше або дорівнює) — повертає true, якщо лівий операнд менше або дорівнює правому. Якщо навпаки, повертає false .

**Оператори рівності**
=

**Оператори несуворої рівності**

console.log(5 == 5); // true
console.log(5 == 3); // false
console.log(5 != 3); // true
console.log(5 != 5); // false

Але є одна проблема!

console.log(5 == "5"); // true
console.log(5 != "5"); // false
console.log(1 == true); // true
console.log(1 != true); // false
Тому краще не порівнбвати значення різних типів!

**Оператори суворої рівності**

console.log(5 === 5); // true
console.log(5 === "5"); // false
console.log(5 !== "5"); // true
console.log(5 !== 5); // false
console.log(1 === true); // false
console.log(1 !== true); // true

**Перетворення типів: числа**
=

**Явне перетворення типів**

console.log(Number("5")); // 5
console.log(Number(true)); // 1
console.log(Number(false)); // 0
console.log(Number(null)); // 0

console.log(Number(undefined)); // NaN
console.log(Number("Jacob")); // NaN
console.log(Number("25px")); // NaN

**Перетворення рядків у числа**
=

Метод Number.parseInt()

console.log(Number.parseInt("5")); // 5 
console.log(Number.parseInt("5.5")); // 5 
console.log(Number.parseInt("5cm")); // 5 
console.log(Number.parseInt("12qwe74")); // 12 
console.log(Number.parseInt("12.46qwe79")); // 12 
console.log(Number.parseInt("cm5")); // NaN 
console.log(Number.parseInt("")); // NaN 
console.log(Number.parseInt("qweqwe")); // NaN

Метод Number.parseFloat()

console.log(Number.parseFloat("5")); // 5
console.log(Number.parseFloat("5.5")); // 5.5
console.log(Number.parseFloat("3.14")); // 3.14
console.log(Number.parseFloat("5cm")); // 5
console.log(Number.parseFloat("5.5cm")); // 5.5
console.log(Number.parseFloat("12qwe74")); // 12
console.log(Number.parseFloat("12.46qwe79")); // 12.46
console.log(Number.parseFloat("cm5")); // NaN
console.log(Number.parseFloat("")); // NaN
console.log(Number.parseFloat("qweqwe")); // NaN

**Арифметичні функції**
=

Клас Math є вбудованим класом JavaScript

Math.floor(num): повертає найближче ціле число, яке є меншим або дорівнює вказаному числу num
Math.ceil(num): повертає найближче ціле число, яке є більшим, або дорівнює зазначеному числу num
Math.round(num): повертає значення числа після округлення до найближчого цілого
Math.max(num1, num2, ...): повертає найбільше число з набору переданих чисел
Math.min(num1, num2, ...): повертає найменше число з набору переданих чисел
Math.random(): повертає випадкове число в діапазоні від 0 (включно) до 1 (за винятком)

**Оголошення та виклик функції**
=

<img width="252" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/92b432e8-49d0-4420-a03f-03f5125333bc">

Ключове слово function
Ім'я функції — це дієслово, що відповідає на питання "Що зробити?"
Пара круглих дужок ()
Тіло функції у фігурних дужках {}


// Оголошення функції multiply
function doStuff() {
  // Тіло функції
  console.log('Log inside multiply function');
}

// Виклики функції multiply
doStuff(); // 'Log inside multiply function'
doStuff(); // 'Log inside multiply function'
doStuff(); // 'Log inside multiply function'

**Параметри та аргументи**
=

**Параметри** - це локальні змінні, доступні лише всередині тіла функції

**Аргументи** - під час виклику функції в круглих дужках можна передати аргументи, які є значеннями для оголошених параметрів функції

<img width="465" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c172ac6d-b297-4aac-a93c-d93ae61c3aa5">

**Повернення значення**
=

function multiply(x, y, z) {
	const product = x * y * z;
  // Повертаємо результат виразу множення
  return product;
}

// Результат роботи функції можна зберегти у змінну
const result = multiply(2, 3, 5);
console.log(result); // 30

**Область видимості функції**
=

// Глобальна змінна
const value = "I'm a global variable";

function foo() {
// Можна звернутися до глобальної змінної
	console.log(value); // "I'm a global variable"
}

foo();
// Можна звернутися до глобальної змінної
console.log(value); 
// "I'm a global variable"

===

function foo() {
	// Локальна змінна
	const value = "I'm a local variable";
	// Можна звернутися до локальної змінної
	console.log(value); // "I'm a local variable"
}

foo();
  console.log(value); // ReferenceError: value is not defined
                      // Помилка: локальну змінну не видно за межами  
                         функції

**Блокова область видимості**
=

![1a13655a-f84e-4561-b73b-19e0fde08a7dFrame 48587 (1)](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/d05942df-1299-49bf-ad5d-c010d7e64773)


**Масиви**
=

Масив — це впорядкована структура даних, яка використовується для зберігання колекції елементів. Масиви можуть містити елементи різних типів даних, таких як числа, рядки, булеві значення тощо.

Для створення масиву в JavaScript використовується літерал масиву: квадратні дужки []. Усередині дужок перераховуються елементи масиву, розділені комами.

Щоб отримати доступ до значення елемента масиву, ми використовуємо синтаксис квадратних дужок:
arrayName[index]

Довжина масиву, тобто кількість його елементів, зберігається у властивості length. Це динамічна величина, яка автоматично змінюється під час додавання або видалення елементів.

Щоб знайти значення останнього елемента масиву, нам потрібно знати його індекс. Індекс останнього елемента можна визначити за допомогою формули довжина_масиву -1.

**Функції частина 2**
=

**Псевдомасив arguments**

Доступ до списку всіх аргументів можна отримати за допомогою спеціальної змінної arguments

<img width="314" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/22d0e8a7-e906-4e3f-8d9c-cc6bf9ae9a52">

Ця колекція схожа на масив, але насправді є псевдомасивом, тобто:

- у неї є деякі властивості масивів, наприклад length
- у неї є можливість звернутися до елемента за індексом
- у неї немає методів для роботи з масивом
- її можна перебирати за допомогою циклів

**Параметри за замовчуванням**
=

Функції можуть мати параметри зі значеннями за замовчуванням, тобто необов'язкові параметри. Ці значення використовуються в тому випадку, якщо функція викликається без передавання відповідного аргументу для цього параметра. Значенням за замовчуванням може бути будь-який тип даних.

<img width="444" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a5a7c532-2d1c-4118-831d-1a10db3f55ca">

**Функціональний вираз**
=

Функціональний вираз (function expression) — звичайне оголошення змінної, значенням якої буде функція. Це альтернативний спосіб оголошення функції.

<img width="459" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/5567ca55-723e-442e-a2e0-c5619c2c54cc">

**Стек викликів**
=

<img width="692" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/80a53850-2e0c-4103-a6f3-398abca4bb4d">

**Stack frame (кадр стека, запис стека)** — структура, яка додається на стек при виклику функції. Зберігає службову інформацію, наприклад ім'я функції та номер рядка, у якому стався виклик.

<img width="269" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/cb519561-7db7-4720-b197-02af16a7872a">

**Об’єкти**
=

**Створення об'єкта**

<img width="526" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/98a87ddf-aa15-4f28-b620-6ef4bccbe09e">

- Для оголошення об’єкта використовуються фігурні дужки {} — літерал об'єкта.
- При створенні об'єкта до нього відразу можна додати властивості, але це не обов’язково. Кожна властивість обов’язково складається з пари ключ: значення.
- Ключ також називають ім'ям властивості і це зазвичай рядок.
- Значенням властивості можуть бути будь-які типи: примітиви, масиви, об'єкти, булі, функції тощо.
- Властивості між собою розділяються комою.

**Вкладені властивості**

<img width="297" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/20e81bc8-f12b-4a2d-84e3-efa9a13f5d51">

**Масив об’єктів**
=

<img width="513" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/19a16efb-0866-4746-8b56-361d0aecad79">

**Методи об'єкта**
=

Об'єкти можуть зберігати не тільки дані, але й функції для роботи з цими даними. Якщо значення властивості — це функція, така властивість називається методом об'єкта.

<img width="586" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/8269f9e1-e529-4ffb-8a7b-eaf30b309296">

**Доступ до властивостей об'єкта**
=

<img width="662" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/472a3283-f860-40ba-8e21-f3226b49e3f6">

Значенням this буде посилання на об'єкт перед «крапкою», тобто об'єкт, який викликав цей метод, у нашому випадку — це посилання на об'єкт bookShelf.

Для доступу до властивостей об'єкта в методах звертаємось до нього через this і далі, стандартно, «через крапку» до властивостей.

<img width="712" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/0dc7011f-607c-4258-a0df-8aa2f9d3393d">

**Синтаксис spread і rest**
=

**Залишкові параметри**

Починаючи зі стандарту ES6, з'явилася концепція залишкових параметрів (...rest). Це спеціальний синтаксис, який дозволяє зібрати групу незалежних елементів у масив.

<img width="435" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e3dbce95-e350-4293-a2d8-92e98b312603">

**Збір частини аргументів**

Операція (...rest) також дозволяє зібрати в масив тільки ту частину аргументів, яка необхідна. Для цього потрібно оголосити параметри до «збирання». Можна покласти перші кілька параметрів у змінні, а решту — зібрати в масив.

<img width="505" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f58aadb5-f98e-49b8-914a-85e8baa131b9">

**Входження параметрів**

<img width="592" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7320e1e0-cf17-4e27-96ab-52f809d38d6a">

<img width="710" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/cb82dd68-0530-4917-b78a-b672d5118fa2">

**Створення масиву**

Операція ...spread дозволяє створити копію масиву або «склеїти» довільну кількість масивів в один новий. Досі для цього використовувалися методи slice() і concat(), але операція розпилення дозволяє зробити те саме в коротшій формі.

<img width="554" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/52ac82c1-2191-4f3b-8d0f-fd7d1cdb1416">

**Створення об'єкта**

<img width="660" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/cb94dc1d-3e32-45f8-b16d-cf3f8def8468">

Порядок розподілу має значення. Імена властивостей об'єкта — унікальні, тому властивості об'єкта, що розпиляються, можуть перезаписати значення вже існуючої властивості, якщо їх імена збігаються.

<img width="710" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/dcdd3e8a-592d-47e7-ba21-86f729322e33">

**Колбек-функції**
=

**Функція як значення**

Значення функції (посилання на неї) можна зберігати у змінній або передавати в якості аргументу в іншу функцію. У цьому сенсі функції не відрізняються від чисел, рядків або масивів.

<img width="683" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/065cba8d-10f8-445a-8517-2e6627f2cf67">

**Колбек-функції**

<img width="711" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7a04fcb0-cff3-4463-9c30-485df54f3707">

**Інлайн-колбеки**

<img width="667" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/b3ff7a33-a59c-4837-b4cd-f4cd6aa2569f">

**Стрілочні функції**
=

**Стрілочні функції: синтаксис**

<img width="404" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/ebdca50f-b5d3-4a84-9e38-cd3b24d54d3f">

**Неявне повернення**

<img width="402" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3ffc0d95-3b24-40ed-97e5-131801335193">

**Псевдомасив arguments**

У стрілочних функцій немає локальної змінної arguments, що містить усі аргументи. Якщо необхідно зібрати всі аргументи в масив, використовується операція rest.

<img width="330" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/0d82eda0-77d7-4820-88e9-4b0b0b747adf">

**Колбеки**

Стрілочну колбек-функцію також можна оголошувати окремо й передавати на неї посилання. Це варто робити, якщо одна функція використовується в декількох місцях програми або якщо вона громіздка.

<img width="563" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3e96a130-fcd0-4c2b-a6d9-002d59b0b97d">

**Методи map і flatMap**
=

**Функція з побічними ефектами** — це функція, яка в процесі виконання може:

- змінювати або використовувати глобальні змінні
- змінювати значення аргументів посилального типу
- виконувати операції введення-виведення тощо

<img width="627" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3ab047c0-4b9b-470f-b852-9d0d848c6ef2">

**Чиста функція (pure function)** — це функція, результат якої залежить тільки від значень переданих аргументів. За умови однакових аргументів вона завжди повертає один і той самий результат і не має побічних ефектів, тобто не змінює значення аргументів.

<img width="600" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/42eb8df5-b7d8-4fac-a4a9-02c281ed0c47">

**Перебираючі методи**

<img width="593" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3067ada6-85b7-43d1-aad5-f184305f2f96">

У більшості методів колбек-функції, які є їхнім аргументом, отримують три наступні параметри:

- першим параметром буде значення поточного елемента масиву currentValue
- другим параметром буде індекс поточного елемента масиву index
- третім параметром буде посилання на сам вихідний масив array

**Контекст виконання функції**
=

**Ключове слово this**

<img width="709" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/630d4c28-31bf-46bf-bf10-0e6abc8762e9">
<img width="565" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/15d92118-db7a-4d8f-868a-bb846d558596">

**Глобальний контекст**

У визначенні значення this є важливий нюанс. Значення this визначається не на момент оголошення функції (за винятком стрілкових функцій), а на момент її виклику. Іншими словами, this визначається тим, як саме функцію викликали, а не де вона була оголошена.

У глобальному контексті, якщо функція виконується не в суворому режимі, this посилається на об'єкт window. Об'єкт window надає доступ до браузерних властивостей і функцій та є глобальним контекстом виконання для скриптів у браузері.

<img width="247" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/4cace3c3-d97a-419b-ac5d-7a21152603ee">

У суворому режимі значення this у глобальному контексті завжди буде undefined.

<img width="245" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/97fae398-64ae-4c52-8fe2-b2f9533462b5">

**Прототипи**
=

У функцій є різні методи, ссе це можливо завдяки механізму прототипного успадкування, який дає змогу організувати об'єкти в ланцюжки таким чином, щоб здійснювався автоматичний пошук властивості в іншому об'єкті, якщо її не знайдено в поточному.

<img width="602" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7e6cbcc1-8812-4aad-9676-cfa4159fc0eb">

**Ланцюжки прототипів**

<img width="752" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/09d7e6aa-3ee8-4c81-bac2-01bf52cde52c">

<img width="725" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/8d5cd94b-0c93-4851-8ab2-a02f72cacf8c">

**ООП**
=

**Процедурне програмування**

Процедурне програмування — це парадигма програмування, у якій програми структуровані у вигляді набору функцій, які виконують певні дії над даними. Основні концепції включають:

- *Процедури (функції)*: Основною одиницею програми є функції. Вони призначені для виконання конкретних завдань. Функції приймають аргументи (вхідні дані), обробляють їх і можуть повертати результат (вихідні дані).
- *Локальні та глобальні змінні*: Змінні, що оголошуються в межах функції, є локальними й доступними лише в цій функції. Змінні, оголошені поза функціями, є глобальними й доступними в усій програмі.

Цей підхід — простий і прямолінійний. Він може використовуватись для задач, в яких немає тісно пов'язаних сутностей (даних і функцій для їх обробки).

<img width="413" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/be186683-735b-4457-938a-ccd1ed3210a2">

Процедурне програмування — це те, як ми з тобою писали код до сих пір. Воно є простим і зрозумілим і може бути використане для написання простих програм. Проте зі збільшенням складності програми процедурний підхід може стати неефективним, оскільки втрачається зв'язок між даними й методами їх обробки.

**Об'єктно-орієнтоване програмування**

Об'єктно-орієнтоване програмування (ООП) — це парадигма програмування, в якій програми структуровані як сукупність об'єктів. Ці об’єкти представляють реальні або абстрактні сутності: користувач, магазин, автомобіль тощо. Кожен з об’єктів містить дані (властивості) і методи для взаємодії з ними.

<img width="533" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/bb08f735-9c69-47e2-a701-aaff7da1bc67">

**!** При такому підході відсутні або майже відсутні глобальні змінні. Методи не залежать від параметрів, а використовують властивості об'єкта, які задаються при його створенні і можуть бути змінені іншими методами.


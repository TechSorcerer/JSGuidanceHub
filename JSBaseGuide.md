
====================================**Базова термінологія**====================================

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

====================================**Підключення скрипта**====================================

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

====================================**Суворий режим**====================================

'use strict';

// Код у суворому режимі

-!- Рекомендується завжди використовувати суворий режим у своїх проєктах, щоб уникнути непередбачуваних ситуацій і проблем у коді.

====================================**Виведення даних**====================================

<img width="733" alt="0656e9d3-94d1-4cba-aba5-8ad39abb85dbScreenshot 2023-07-04 at 16 51 35" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a2a15a15-3364-46da-9ba4-0d8e5b3d40d6">

Наступні комбінації клавіш відкривають інструменти розробника на вкладці Console:
Windows і Linux — Ctrl + Shift + J;
MacOS — Command + Option + J .

Щоб вивести дані в консоль розробника використовується метод console.log()

console.log("JavaScript is awesome!");
console.log(10);

<img width="662" alt="2e0efa32-9ccb-4dcc-80b3-46d0ea254b72Screenshot 2023-07-04 at 16 58 55" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/726b585b-eba3-4469-b0bd-3a8c690848e1">

====================================**Оголошення змінних**====================================

let age = 20 
const username = "Mango"

Ключове слово (let / const) => назва змнної (age, username (може буьт будь-яка)) => змінна (20, "Mango")

====================================**Перевизначення змінних**====================================

<img width="424" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f26196cb-861c-437d-9d2f-9ec2581cde0f">

Змінну let можна змінити, змінну const - ні!

<img width="636" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e0fb1df1-06c7-4c97-8a7b-a79ac873af07">

====================================**Найменування**====================================

<img width="279" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f8e65e21-ad2e-434a-80d9-9f41907e303f">

Варто пам'ятати, що існують зарезервовані **ключові слова**

![9f4e2b98-8e94-46de-a640-f03c05f39327m01-b02-s04](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/2280e368-0b19-465b-84cd-bc91c168fbdb)

====================================**Типи даних**====================================

**Number**

const age = 20;
const salary = 3710.84;

**String**

const username = 'Mango995';
const description = "JavaScript is awesome!";

**Boolean**

const isModalOpen = true;
const isLoggedIn = false;

====================================**Спеціальні значення**====================================

let value = null;
console.log(value); // null

let value;
console.log(value); // undefined

Хоча обидва значення null і undefined позначають відсутність значення, вони мають трохи різні семантики використання.
 — null використовується для явної вказівки порожнього значення (точно відомо, що значення немає).
 — undefined вказує на невизначеність значення змінної.

====================================**Оператор typeof**====================================

typeof operand - Замість operand ти вказуєш змінну, літерал або вираз, тип якого ти хочеш визначити. Результатом оператора typeof буде рядок, який вказує тип даних.

====================================**Арифметичні операції**====================================

<img width="340" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c835dee6-c5f0-4490-90a6-f393c18ba1c5">

Оператор (+) використовується для складання двох чисел.
Оператор (-) використовується для віднімання одного числа від іншого.
Оператор (*) використовується для множення двох чисел.
Оператор (/) використовується для ділення одного числа на інше.
Оператор (%) повертає остачу від ділення одного числа на інше.
Оператор (**) використовується для піднесення числа до степеня.

====================================**Комбіновані оператори**====================================

Додавання: +=. Приклад: x += y еквівалентно x = x + y

Віднімання: -=. Приклад: x -= y еквівалентно x = x - y

Множення: *=. Приклад: x *= y еквівалентно x = x * y

Ділення: /=. Приклад: x /= y еквівалентно x = x / y

Остача від ділення: %=. Приклад: x %= y еквівалентно x = x % y

====================================**Конкатенація рядків**====================================

Якщо застосувати оператор + до рядка та будь-якого іншого типу даних, результатом буде новий рядок, що містить об'єднання вихідних значень.

const message = "Mango " + "is" + " happy";
console.log(message); // "Mango is happy"

console.log("Mango" + 55); // "Mango55"
console.log("Mango" + true); // "Mangotrue"

console.log(1 + "2"); // "12"
console.log(1 + "2" + 4); // "124"
console.log(1 + 2 + "4"); // "34"

====================================**Перетворення типів: рядки**====================================

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

====================================**Шаблонні рядки**====================================

Шаблонні рядки огортаються зворотними лапками (англ. backticks) (``)

Увага! 
Код не працюватиме, якщо огорнути шаблонні рядки звичайними одинарними або подвійними лапками.

====================================**Довжина рядка**====================================

Для доступу до властивості (property) сутності (objectName) використовується синтаксис із крапкою:
сутність.властивість

У програмуванні, наприклад, рядок має властивість length, яка повертає довжину рядка.

const productName = "Repair droid";

// Якщо у змінній зберігається рядок
console.log(productName.length); // 12

// Якщо рядковий літерал
console.log("Repair droid".length); // 12

====================================**Індексація рядків**====================================

![72eb24ab-b422-4ed8-afb7-1c03955121d7m01-b03-s06](https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/bc1dd07b-5212-4269-9b92-ec2c1091226b)

====================================**Оператори порівняння**====================================

Оператор > (більше) — повертає true, якщо лівий операнд більше правого. В іншому разі повертає false .

Оператор < (менше) — повертає true, якщо лівий операнд менше правого. В іншому разі повертає false .

Оператор >= (більше або дорівнює) — повертає true, якщо лівий операнд більше або дорівнює правому. Якщо навпаки, повертає false .

Оператор <= (менше або дорівнює) — повертає true, якщо лівий операнд менше або дорівнює правому. Якщо навпаки, повертає false .

====================================**Оператори рівності**====================================

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

====================================**Перетворення типів: числа**====================================

**Явне перетворення типів**

console.log(Number("5")); // 5
console.log(Number(true)); // 1
console.log(Number(false)); // 0
console.log(Number(null)); // 0

console.log(Number(undefined)); // NaN
console.log(Number("Jacob")); // NaN
console.log(Number("25px")); // NaN

====================================**Перетворення рядків у числа**====================================

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

====================================**Арифметичні функції**====================================

Клас Math є вбудованим класом JavaScript

Math.floor(num): повертає найближче ціле число, яке є меншим або дорівнює вказаному числу num
Math.ceil(num): повертає найближче ціле число, яке є більшим, або дорівнює зазначеному числу num
Math.round(num): повертає значення числа після округлення до найближчого цілого
Math.max(num1, num2, ...): повертає найбільше число з набору переданих чисел
Math.min(num1, num2, ...): повертає найменше число з набору переданих чисел
Math.random(): повертає випадкове число в діапазоні від 0 (включно) до 1 (за винятком)

====================================**Оголошення та виклик функції**====================================

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

====================================**Параметри та аргументи**====================================

**Параметри** - це локальні змінні, доступні лише всередині тіла функції

**Аргументи** - під час виклику функції в круглих дужках можна передати аргументи, які є значеннями для оголошених параметрів функції

<img width="465" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c172ac6d-b297-4aac-a93c-d93ae61c3aa5">

====================================**Повернення значення**====================================

function multiply(x, y, z) {
	const product = x * y * z;
  // Повертаємо результат виразу множення
  return product;
}

// Результат роботи функції можна зберегти у змінну
const result = multiply(2, 3, 5);
console.log(result); // 30

====================================**Область видимості функції**====================================

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


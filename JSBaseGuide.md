
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


let username = "Mango";
console.log(username); // "Mango"

username = "Poly";
console.log(username); // "Poly"


const username = "Mango";
console.log(username); // "Mango"

// ❌ Неправильно, буде помилка
username = "Poly"; // TypeError: Assignment to constant variable.

Змінну let можна змінити, змінну const - ні!

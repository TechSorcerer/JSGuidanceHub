**Перетворення рядків у числа** 
=

Number.parseInt() 

<img width="552" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/967bb5cf-b4d2-4474-b524-7da4498db9b8">

Number.parseFloat()

<img width="605" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/4ae5a920-8992-4827-b21d-273405f8f803">

**Інструкція if**
=

<img width="368" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c2ca251c-cc8c-434b-add7-ba6d1f1133ad">

**Інструкція if...else**
=

<img width="501" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e82f0492-6d60-4dc2-bb7c-02785c6629a6">

**Блок else...if**
=

<img width="605" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7508d9c9-0895-476c-b64d-5c2a4217d20d">

**Тернарний оператор**
=

<img width="343" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/65b23d72-0217-44d6-a44b-68bbb84e8bf4"> ==> <img width="492" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/d1f3fdab-9192-4174-b8ce-23284f84f129">

Тернарний оператор рекомендується використовувати у найпростіших випадках операції присвоєння чи повернення. 
Однак не рекомендується використовувати його для складних розгалужень, оскільки це може ускладнити читання та розуміння коду.

**Оператор switch**
=

switch (expression) {
  case value1:
    // код, що виконується, якщо вираз (expression) дорівнює value1
    break;
  case value2:
    // код, що виконується, якщо вираз (expression) дорівнює value2
    break;
  // ...
  default:
    // код, що виконується, якщо вираз (expression) не відповідає жодному значенню
}

<img width="570" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c3397b48-239b-495c-9341-0f2b7c6d507a">

**Оператор break**
=

Після виконання коду в одному з випадків потрібно використовувати оператор break, щоб вийти з оператора switch.

Якщо break не вказано, виконання коду продовжиться в наступному case і далі. Така поведінка називається "провалюванням" (fall-through). Якщо потрібно, щоб кілька блоків case виконували той самий код, можна опустити оператор break між ними.

const day = 3;

switch (day) {
  case 1:
  case 2:
  case 3:
  case 4:
  case 5:
    console.log('This is a working day');
    break;
  case 6:
  case 7:
    console.log('It is a day off');
    break;
  default:
    console.log('Invalid');
}

**Логічне «І»**
=

Логічні оператори використовуються для перевірки умов з кількома виразами, наприклад, в інструкції if.

Оператор "І" (&&) наводить усі операнди до логічного типу (true або false) і повертає значення одного з них. Дозволяє перевірити, чи виконані всі умови у виразі.

**Оператор “І” зліва направо перевіряє почергово обидва операнди на істинність та повертає або значення останнього істинного (тільки правого) операнда, або першого хибного (лівого чи правого), на якому він запнувся**

**Логічне «АБО»**
=

Оператор "АБО" (||) перетворює всі операнди до логічного типу (true або false) і повертає значення одного з них.

Дозволяє перевіряти, чи є хоча б один із операндів "істинним”.
Обчислення оператора відбувається зліва направо.

**Якщо хоча б один із операндів можна перетворити на true, результатом логічного «АБО» буде цей операнд.**

**Якщо всі операнди перетворюються на false, результатом буде значення крайнього правого операнда.**

**Логічне «НІ»**
=

Логічне «НІ» (!) — це унарний оператор — він виконує операцію над одним операндом праворуч.

Логічне «НІ» приводить операнд до логічного значення (true або false) і потім заперечує (інвертує) його, тобто заміняє на протилежне: true —> false, а false —> true.

**Метод slice()**
=

str.slice(startIndex, endIndex) - Метод slice() копіює підрядок із вихідного рядка, починаючи з індексу startIndex і до (не включаючи) індексу endIndex, і повертає цю копію як новий рядок.

<img width="654" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/99906833-890f-4133-bf40-da6a92287132"> 

Параметр endIndex є необов'язковим. Якщо endIndex не вказаний, витягуються всі елементи до кінця рядка.
Якщо викликати метод slice() без аргументів, він створює точну копію рядка і повертає її.

**Методи toLowerCase() і toUpperCase()**
=

Метод toLowerCase() повертає новий рядок, у якому всі символи вихідного рядка перетворені в нижній регістр.
Метод toUpperCase() повертає новий рядок, у якому всі символи вихідного рядка перетворені у верхній регістр.

**Метод includes()**
=

Метод рядків includes() використовується для перевірки наявності підрядка у рядку. Він повертає логічне значення true, якщо підрядок знайдено, і false, якщо підрядок відсутній.

str.includes(substring)
де:
str — вихідний рядок, у якому ми шукаємо підрядок;
substring — підрядок, який ми хочемо знайти у вихідному рядку.

**Методи startsWith() і endsWith()**
=

Методи startsWith() і endsWith() призначені для перевірки початку й закінчення рядка відповідно. Вони повертають булеве значення true або false, залежно від того, чи відповідає початок або кінець рядка заданому значенню.

str.метод(substr)
substr — це рядок, з якого має починатися вихідний рядок.

Зверни увагу! 
Обидва методи чутливі до регістру символів. Це означає, що під час порівняння підрядка з вихідним рядком регістр символів має збігатися. Якщо в ці методи не передати аргумент, то він повертає false.

**Метод indexOf()**
=

Метод indexOf() використовується для пошуку першого входження підрядка в рядок. Він повертає:
індекс першого входження (індекс першого символу) підрядка, якщо він знайдений або
-1, якщо підрядок не виявлено

str.indexOf(substr)
str — вихідний рядок, у якому потрібно виконати пошук
substr — рядок, який потрібно знайти у вихідному рядку

**Метод trim()**
=

Метод trim() використовується для видалення початкових і кінцевих пробілів із рядка.

str.trim()

Зверни увагу! 
Метод trim() не змінює вихідний рядок, а повертає новий рядок без початкових і кінцевих пробілів.

**Цикл while**
=

Конструкція while створює цикл, який виконує блок коду в тілі циклу, поки умова для виходу оцінюється як true.

while (condition) {
  statement // код, тіло циклу
}

<img width="292" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/14e4ffd8-9cb1-4fa1-ad3e-89a4c1d2508c">

let count = 0;

while (count < 10) {
  console.log(`Count: ${count}`);
  count += 1;
}

**Цикл do…while**
=

Цикли while і do...while працюють схожим чином, але мають одну ключову відмінність. Під час використання циклу do...while код у тілі циклу виконується принаймні один раз, навіть якщо умова не виконується з самого початку.

do {
   statement // код, який буде виконуватися
} while (condition);

let count = 0;

do {
	console.log(`Count: ${count}`);
	count += 1;
} while (count < 5);

**Цикл for**
=

for (initialization; condition; afterthought) {
  statement // Тіло циклу
}

Ініціалізація — виконується один раз перед початком циклу. Тут оголошується змінна-лічильник і вказується її початкове значення.
Умова — це вираз, який оцінюється перед кожною ітерацією (повторенням) циклу. Якщо умова перетворюється на**true**, то виконується тіло циклу. Якщо умова перетворюється на false, то цикл завершується.
Пост-вираз — це вираз, який виконується в кінці кожної ітерації циклу, перед перевіркою умови. Використовується для оновлення значення змінної-лічильника.
Тіло циклу — це блок коду, який буде виконуватися на кожній ітерації циклу, якщо умова перетворюється на true.

<img width="642" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/77657f06-fe77-422a-bce2-23b58ac150b3">

for (let i = 0; i <= 20; i += 5) {
  console.log(i);
}

**Інкремент**
=

Префіксний інкремент (++value) спочатку збільшує значення змінної, а потім використовує нове значення у виразі.
let x = 5;
const y = ++x;
console.log(x); // 6
console.log(y); // 6

Постфіксний інкремент (value++) спочатку використовує поточне значення змінної у виразі, а потім виконує збільшення значення.
let x = 5;
const y = x++;
console.log(x); // 6
console.log(y); // 5

**Декремент**
=

Префіксний декремент (--value) спочатку зменшує значення змінної, а потім використовує нове значення у виразі.
let x = 5;
const y = --x;
console.log(x); // 4
console.log(y); // 4

Постфіксний декремент (value--) спочатку використовує поточне значення змінної у виразі, а потім виконує зменшення значення.
let x = 5;
const y = x--;
console.log(x); // 4
console.log(y); // 5

for (let i = 0; i <= 5; i++) {
  console.log(i);
}

**Методи масивів**
=

**Метод join()**

<img width="649" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/6439df50-bd65-4711-aa19-22818f08c5b6">

**Метод split()**

<img width="693" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/6b4a3932-6848-42cc-bb57-c8914d200dbf">

**Метод slice()**

<img width="706" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/d5f00875-1f3e-4e68-ace5-e2084d25882f">

**Метод concat()**

<img width="605" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c9d9b944-ab0f-49a8-a9f6-474750265489">

**Метод indexOf()**

array.indexOf(elem)

<img width="669" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/f1638e7b-1474-46e0-a033-12e2ba9d00a6">

**Метод push()**

<img width="709" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3c37c0e3-fedb-40a2-994f-d4c7338fd154">

**Метод includes()**

array.includes(element)

<img width="602" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/85b5d694-b360-48d3-a3a1-b197e3a53662">

**Обʼєкти**
=

**Доступ до властивостей обʼєкта через крапку**

<img width="699" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/b53f9022-1491-495d-bd23-27fee7de6304">

**Доступ до вкладених властивостей**

<img width="662" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/4e61930d-1ef6-425a-833e-38b0a265c9d8">

**Доступ до властивостей через квадратні дужки**

<img width="707" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/d762e524-8f13-4da9-b082-4df4b94caba1">

**Зміна значення властивостей**

<img width="703" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e6240708-3e8d-4fa4-b7e5-8aadbc3b4f14">

**Додавання властивостей**

<img width="578" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/97aabb6c-0481-466f-a1fe-22353b5d15a3">

**Короткі властивості**

<img width="477" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/b5283a81-2174-45a3-a604-ead4afeb4e91">

**Обчислювальні властивості**

<img width="697" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e766f504-9898-42ed-a936-6e285b6e1fc9">

**Перебір об'єкта**
=

**Цикл for...in**

for (key in object) {
  // інструкції
}

<img width="669" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/1ca9db37-1121-4ec6-859d-848552d5db81">

**Метод Object.keys()**

<img width="693" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c2647a0a-b10f-45e0-b167-289a7738403c">

**Метод Object.values()**

<img width="636" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/5966c95e-b26e-428b-b9f4-bf78d97110a4">

**Колбек-функції**
=

**Метод forEach(callback)**

Метод forEach(callback) — це метод перебирання масиву, який використовується для заміни циклів for і for...of в роботі з колекцією.

array.forEach(function callback(element, index, array) {
  // Тіло колбек-функції
});

<img width="583" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/dd6c75c0-9910-42eb-9265-46631fd4afb3">

**Методи map і flatMap**
=

**Метод map()**

array.map((element, index, array) => {
  // Тіло колбек-функції
});

- Поелементно перебирає оригінальний масив
- Не змінює оригінальний масив
- Результат роботи колбек-функції записується в новий масив
- Повертає новий масив такої ж довжини, як і в масиву, до якого він був застосований

<img width="707" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e613f45d-55fd-4102-b9ad-e2b89c3565ac">

**Метод flatMap()**

Метод flatMap(callback) аналогічний методу map(), але застосовується у випадках, коли результат — це багатовимірний масив, який необхідно «розгладити».

array.flatMap((element, index, array) => {
  // Тіло колбек-функції
});

<img width="711" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/083a60ca-152a-4251-9ca3-2418658d52cc">

**Метод filter() на масиві об'єктів**

<img width="695" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/99c89a6c-fad8-4ff6-bd89-0ce178874769">

**Метод find()**

Ти вже знаєш, що метод filter(callback) використовується для пошуку всіх елементів, що задовольняють умову.

Метод find(callback) дозволяє знайти і повернути перший відповідний елемент, що задовольняє умову, після чого перебирання масиву припиняється. Тобто він, на відміну від методу filter(callback), шукає до першого збігу.

<img width="713" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/326a70f6-d900-4ebe-b1d5-fb98254b1fec">

**Метод every()**

array.every((element, index, array) => {
  // Тіло колбек-функції
});

- Не змінює оригінальний масив
- Поелементно перебирає оригінальний масив
- Повертає true, якщо всі елементи масиву задовольняють умову
- Повертає false, якщо хоча б один елемент масиву не задовольняє умову
- Перебирання масиву припиняється, якщо колбек повертає false

<img width="673" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/95cd780a-0199-4869-9885-d5cb72b35403">

**Метод some()**

- Не змінює оригінальний масив
- Поелементно перебирає оригінальний масив
- Повертає true, якщо хоча б один елемент масиву задовольняє умову
- Повертає false, якщо жоден елемент масиву не задовольняє умову
- Перебирання масиву припиняється, якщо колбек повертає true

<img width="694" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/8b1420c1-d6c7-47ed-ac8d-0f1d56cbfdbf">

**Метод reduce()**

array.reduce((previousValue, element, index, array) => {
  // Тіло колбек-функції
}, initialValue);

- Не змінює оригінальний масив
- Поелементно перебирає оригінальний масив
- Повертає все, що завгодно (об’єкт, масив, рядок, число тощо)
- Може замінити функціонал будь-якого іншого перебираючого методу масиву та навіть їх комбінацію

<img width="677" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/1ec35158-b9eb-4d19-b52d-6dfa34eea0c8">

**Метод reduce() і масив об'єктів**

<img width="687" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3f427056-6003-4c7c-bf88-c579b1f7d7ed">

**Метод toSorted()**
=

array.toSorted();

- Сортує вихідний масив
- Повертає новий масив
- За замовчуванням сортує за зростанням

**Свій порядок сортування чисел**

array.toSorted((a, b) => {
  // Callback function body
});

a — перший елемент для порівняння.
b — другий елемент для порівняння.

*Сортування за зростанням*

<img width="650" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a32bf198-8a88-4a75-80fd-4047501b896e">

*Сортування за спаданням*

<img width="656" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a14db28b-4421-4b77-a58c-bb4f2a9e08bc">

**Свій порядок сортування рядків**

firstString.localeCompare(secondString)

Він викликається на рядку, який потрібно порівняти (firstString) з тим, що був переданий йому як аргумент (secondString).

<img width="695" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/01f45372-a3c6-4139-9c8f-08cf800d4001">

**Контекст виконання функції**
=

**Метод call()**

foo.call(thisArg, arg1, arg2, ...)

- thisArg — об'єкт, який ми хочемо встановити як контекст (значення this) для функції
- arg1, arg2, ... — необов'язкові аргументи, які будуть передані функції

<img width="640" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/42f29bed-eded-43d3-895d-6b95a9389993">

За допомогою методу call ми можемо викликати функцію greet так, щоб значення this вказувало на потрібний об'єкт і використовувало значення його властивостей.

<img width="712" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/6d2d1af2-0c96-4185-a7c1-4f4e590e8481">

**Метод apply()**

foo.apply(thisArg, [arg1, arg2, ...])

- thisArg — об'єкт, який ми хочемо встановити як контекст (значення this) для функції.
- arg1, arg2, ... — необов'язкові аргументи, які будуть передані функції.

<img width="715" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/33b83202-99a9-48d1-9c82-f2a427eb287c">

**Метод bind() і втрата контексту**

Методи call і apply викликають функцію «на місці», тобто одразу.
Метод bind створює і повертає нову функцію, яка має заздалегідь встановлений контекст, і ця нова функція може бути викликана пізніше з будь-якими аргументами.

const boundFoo = foo.bind(thisArg, arg1, arg2, ...)

- thisArg — об'єкт, який ми хочемо встановити як контекст (значення this) для функції
- arg1, arg2, ... — необов'язкові аргументи, які будуть передані функції при її виклику

<img width="554" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/a2ad3017-b875-46fa-9d15-a1a51cb04d0e">

**Метод bind() і колбеки**

Розглянемо приклад втрати контексту, коли ми передаємо метод об'єкта як колбек-функцію:

<img width="701" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7274d270-d5bf-41ce-a592-3ebfa3341899">

Щоб уникнути цієї втрати контексту, можна використати метод bind(). Замість передачі оригінального методу getFullName, ми передаємо його копію, до якої прив'язаний контекст об'єкта customer.

<img width="707" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c5abec6b-08e3-496d-9202-cf4968c71814">

**Алгоритм визначення this**
=

<img width="777" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e5f39be9-e5e8-434a-abc3-44ef9eb9e325">

**Прототипи**
=

**Метод Object.create(obj)**

- створює і повертає новий об'єкт, зв'язуючи його з об'єктом obj.

<img width="693" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/48f5e4bd-9928-4e81-ba94-fa6da203ace9">

**Перевірка прототипу**

objA.isPrototypeOf(objB)

- Метод перевіряє, чи є об'єкт objA прототипом для об’єкта objB
- Якщо так, повертає true, в іншому разі повертає false

<img width="705" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/8bb83945-3185-4c6a-a1d8-c7ff59abb1c1">

**Власні і невласні властивості**

Для того щоб перевірити, чи є в об'єкті власна властивість, використовується метод obj.hasOwnProperty(key). Цей метод перевіряє наявність власної властивості з ім'ям key і повертає true, якщо є, і false в іншому випадку.

<img width="602" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/73a4a539-c817-4594-85e6-64388068b214">

**Перебір власних властивостей**

Для вибору саме власних властивостей під час перебору циклом for...in необхідно на кожній ітерації додати перевірку на власну властивість методом obj.hasOwnProperty(key). Цей метод повертає true, якщо властивість з іменем key належить об'єкту obj, а не його прототипу, в іншому разі — false. Розгляньмо приклад:

<img width="465" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/00fd7e22-d4ce-4bc6-990a-986c15a05d40">

- Якщо це власна властивість — виконуємо тіло if
- Якщо це невласна властивість — нічого не робимо

Методи *Object.keys(obj)* і *Object.values(obj)* повертають масив тільки власних ключів або значень тільки власних властивостей об'єкта obj, без необхідності додаткових перевірок. Через це на практиці використовують саме їх із циклом for...of, замість for...in і hasOwnProperty.

<img width="554" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/10e3493f-4139-48d9-89b3-a2ac92b4f5ad">

**Класи**
=

**Оголошення класу**

Оголошення класу має такий синтаксис:

- ключове слово class
- ім’я класу (у прикладі: User)
- тіло класу у фігурних дужках

class User {
  // Тіло класу
}

А як створити з класу екземпляр?

<img width="350" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/b550b581-905a-4ca9-b2e1-38cd8d60d1aa">

**Конструктор класу**

Для ініціалізації екземпляра класу використовується метод constructor.

Якщо його не визначити в явному вигляді, то буде створений конструктор за замовчуванням — порожня функція, яка не змінює екземпляр класу.

<img width="449" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3540f51e-45f7-4d47-8613-eef518b7453b">

**Об'єкт параметрів**

<img width="526" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/e59b8fca-f279-457f-8860-cd9f28abc79a">

**Методи класу**

Методи класу — це функції, які будуть доступні екземпляру в його прототипі. Вони оголошуються в довільному порядку після конструктора. На відміну від синтаксису методів об'єкта (вони розділяються комою), методи класу не розділені жодними спеціальними символами.

<img width="390" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/7fd1fc9f-8852-42f1-9c6e-05a8bc2c2a5c"> <img width="356" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/775c3825-d312-4d80-b3cc-00194f1e3cbf">

**Прототип екземпляру**

Методи класу додаються до спеціального об'єкта, який зберігається у властивості prototype самого класу.

<img width="702" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/b784bf36-89ec-49b4-a550-121c385c74bb">

<img width="721" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/4e03c304-3775-421d-a3ac-6ebc8a63f4f1">

**Приватні властивості**

<img width="681" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/60742b03-a07f-431d-86f1-46eee7faf245">

**Приватні методи**

<img width="639" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/559247e6-5085-4aa2-81e6-45e1f993e1e4">
<img width="698" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/71ebccbd-43c1-4b2f-af28-4fb279f35ca6">

**Геттери і сеттери**

Геттери і сеттери — це спеціальний синтаксис оголошення методів для взаємодії з властивостями. Геттер і сеттер імітують звичайну публічну властивість класу, але дозволяють взаємодіяти з іншими властивостями зручнішим способом.

<img width="440" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3c7d082f-c37d-44cc-9a15-3671b4386515">

*Геттер і сеттер повинні називатися однаково. 
Краще називати геттери і сеттери так само, як і властивість, з якою вони працюють. Геттер може існувати без сеттера, так само як і сеттер без геттера.*

*Геттери і сеттери доречно використовувати для простих операцій читання та зміни значення властивостей, особливо приватних, як їх публічний інтерфейс. Для роботи з властивістю, яка зберігає масив або об'єкт, вони не підійдуть.*

**Статичні властивості**

<img width="476" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/4aac9d0e-7e5c-4ee1-9c00-251827ea1b0e">

У екземпляра немає доступу до статичних властивостей класу.

<img width="474" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/dfea50dd-60d9-423f-97d2-203270d43e8b">

**Статичні методи**

<img width="505" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/65b54c25-8029-4f1f-8862-1e223f61ddc5">

*Особливість статичних методів*
Під час їх виклику ключове слово this посилається на сам клас. Це означає, що статичний метод може отримати доступ до **статичних властивостей класу**, але **не до властивостей екземпляра**. Це логічно, адже статичні методи викликає сам клас, а не його екземпляри.

**Наслідування класів**

Ключове слово extends дозволяє реалізувати наслідування класів, коли один клас (дочірній, похідний) наслідує властивості й методи іншого класу (батьківського).

<img width="350" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/05cd9dee-db91-466d-85f9-837f6c738805">

<img width="778" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/46010907-9786-4242-b875-1af8fa0853ab">

**Конструктор дочірнього класу**

У конструкторі дочірнього класу необхідно викликати спеціальну функцію super(args) — це псевдонім конструктора батьківського класу.

**!!** В іншому випадку при спробі звернутися до this у конструкторі дочірнього класу виникне помилка.

<img width="717" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/3ae309ca-df52-42b5-81c9-afc8b54c1a1f">

**Методи дочірнього класу**

Дочірній клас може використовувати методи та властивості батьківського класу. Крім цього, у дочірньому класі можна оголошувати методи, які будуть доступні тільки його екземплярам.

<img width="703" alt="image" src="https://github.com/TechSorcerer/JSGuidanceHub/assets/136632373/c931ad16-f4fa-4749-9fb8-f4547300dfe7">


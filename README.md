# 📘 Методҳои String дар JavaScript

Дар поён, феҳристи методҳои маъмул ва муҳим барои кор бо сатрҳо (string) дар JavaScript оварда шудааст. Ҳар кадоми онҳо бо мисол ва тавзеҳи фаҳмо шарҳ дода шудаанд.

---

## 1️⃣ `charAt(index)`

📌 **Шарҳ:** Ин метод рамзи дар мавқеи (index) додашударо бармегардонад.

📍 **Мисол:**
```js
let str = "Salom";
console.log(str.charAt(1)); // "a"
2️⃣ at(index)
🧭 Шарҳ: Подобӣ ба charAt() аст, аммо инчунин индексҳои манфиро дастгирӣ мекунад (аз охир ба ҳисоб).

📍 Мисол:

js
let str = "Salom";
console.log(str.at(-1)); // "m"
3️⃣ toString()
🔁 Шарҳ: Объектро ба сатр (string) табдил медиҳад.

📍 Мисол:

js
let num = 123;
console.log(num.toString()); // "123"
4️⃣ concat()
➕ Шарҳ: Сатрҳоро бо ҳам мепайвандад.

📍 Мисол:

js
let a = "Salom";
let b = "Dunyo";
console.log(a.concat(" ", b)); // "Salom Dunyo"
5️⃣ trim()
✂️ Шарҳ: Фосилаҳои иловагии аввали ва охири сатрро пок мекунад.

📍 Мисол:

js
let str = "  Salom  ";
console.log(str.trim()); // "Salom"
6️⃣ includes(substring)
🔍 Шарҳ: Мебинад, ки оё сатр порае (substring) дорад ё не.

📍 Мисол:

js
let str = "Ман код менависам";
console.log(str.includes("код")); // true
7️⃣ indexOf(substring)
📍 Шарҳ: Индекси аввалини пораи ёфтшударо бармегардонад. Агар набошад — -1.

📍 Мисол:

js
let str = "JavaScript";
console.log(str.indexOf("S")); // 4
8️⃣ lastIndexOf(substring)
🔁 Шарҳ: Индекси охирин бор пайдошударо меёбад.

📍 Мисол:

js
let str = "abca";
console.log(str.lastIndexOf("a")); // 3
9️⃣ replace(old, new)
🛠 Шарҳ: Қисме аз сатрро бо дигаре иваз мекунад (фақат аввалин ёфтшударо).

📍 Мисол:

js
let str = "Салом Салом";
console.log(str.replace("Салом", "Hi")); // "Hi Салом"
🔟 replaceAll(old, new)
🧹 Шарҳ: Ҳама пайдоишҳои як substring-ро иваз мекунад.

📍 Мисол:

js
let str = "Салом Салом";
console.log(str.replaceAll("Салом", "Hi")); // "Hi Hi"
1️⃣1️⃣ substring(start, end)
✂️ Шарҳ: Порае аз сатрро байни ду индекс мебарорад.

📍 Мисол:

js
let str = "JavaScript";
console.log(str.substring(0, 4)); // "Java"
1️⃣2️⃣ slice(start, end)
🔪 Шарҳ: Подобӣ ба substring(), вале индексҳои манфиро дастгирӣ мекунад.

📍 Мисол:

js
let str = "JavaScript";
console.log(str.slice(-6)); // "Script"
1️⃣3️⃣ split(separator)
🔧 Шарҳ: Сатрро ба массив табдил медиҳад, бо ҷудокунандаи додашуда.

📍 Мисол:

js
let str = "a,b,c";
console.log(str.split(",")); // ["a", "b", "c"]
1️⃣4️⃣ toLowerCase()
🔤 Шарҳ: Ҳама ҳарфҳоро ба ҳарфҳои хурд (lowercase) табдил медиҳад.

📍 Мисол:

js
let str = "SALOM";
console.log(str.toLowerCase()); // "salom"
1️⃣5️⃣ toUpperCase()
🔠 Шарҳ: Ҳама ҳарфҳоро ба ҳарфҳои калон (UPPERCASE) табдил медиҳад.

📍 Мисол:

js
let str = "salom";
console.log(str.toUpperCase()); // "SALOM"


















# 📘 Методҳои Math ва isNaN дар JavaScript

JavaScript дорои китобхонаи `Math` мебошад, ки як қатор методҳои муфид барои коркарди ададҳоро дар бар мегирад. Дар поён тавзеҳ ва мисолҳои равшан оварда шудаанд. 🔢

---

## 1️⃣ `Math.floor(x)`

📉 **Шарҳ:** Адади касриро ба тарафи поён (ба сӯи 0) ба адади тамом табдил медиҳад.

📍 **Мисол:**
```js
console.log(Math.floor(4.9)); // 4
2️⃣ Math.ceil(x)
📈 Шарҳ: Адади касриро ба тарафи боло (ба сӯи +∞) ба адади тамом мебарад.

📍 Мисол:

js
console.log(Math.ceil(4.1)); // 5
3️⃣ Math.round(x)
⚖️ Шарҳ: Адади касриро ба наздиктарин адади тамом метабдил медиҳад.

📍 Мисол:

js
console.log(Math.round(4.4)); // 4
console.log(Math.round(4.5)); // 5
4️⃣ Math.abs(x)
➕ Шарҳ: Қимати мутлақ (absolute value) яъне мусбии ададро бармегардонад.

📍 Мисол:

js
console.log(Math.abs(-10)); // 10
5️⃣ Math.max(a, b, c, ...)
🔼 Шарҳ: Қимати калонтарини ададҳои додашударо бармегардонад.

📍 Мисол:

js
console.log(Math.max(5, 10, 20)); // 20
6️⃣ Math.min(a, b, c, ...)
🔽 Шарҳ: Қимати хурдтарини ададҳои додашударо бармегардонад.

📍 Мисол:

js
console.log(Math.min(5, 10, 1)); // 1
7️⃣ Math.pow(base, exponent)
🧪 Шарҳ: Адади асос (base)-ро ба дараҷаи муайян (exponent) мебарад.

📍 Мисол:

js
console.log(Math.pow(2, 3)); // 8
// 2^3 = 8
📌 Эзоҳ: Дар ES6 инчунин метавон навишт:

js
console.log(2 ** 3); // 8
8️⃣ Math.sqrt(x)
🧮 Шарҳ: Реша (square root) — решаи квадрати ададро бармегардонад.

📍 Мисол:

js
console.log(Math.sqrt(25)); // 5
9️⃣ Math.random()
🎲 Шарҳ: Рақами тасодуфӣ байни 0 ва 1 (бе дохил кардани 1) месозад.

📍 Мисол:

js
console.log(Math.random()); // 0.5348...
📌 Барои рақами тасодуфии байни 1 то 10:

js
let rand = Math.floor(Math.random() * 10) + 1;
console.log(rand); // 1 то 10
🔟 isNaN(value)
🚫 Шарҳ: Мебинад, ки оё арзиш (value) NaN аст ё не (NaN = Not a Number).

📍 Мисол:

js
console.log(isNaN("hello")); // true
console.log(isNaN(123));     // false
📌 Эзоҳ: isNaN() метавонад баъзан натиҷаи интизорнашударо диҳад, барои дақиқтар санҷидан Number.isNaN()-ро истифода баред.


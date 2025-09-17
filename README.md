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
Копировать код
let str = "Salom";
console.log(str.at(-1)); // "m"
3️⃣ toString()
🔁 Шарҳ: Объектро ба сатр (string) табдил медиҳад.

📍 Мисол:

js
Копировать код
let num = 123;
console.log(num.toString()); // "123"
4️⃣ concat()
➕ Шарҳ: Сатрҳоро бо ҳам мепайвандад.

📍 Мисол:

js
Копировать код
let a = "Salom";
let b = "Dunyo";
console.log(a.concat(" ", b)); // "Salom Dunyo"
5️⃣ trim()
✂️ Шарҳ: Фосилаҳои иловагии аввали ва охири сатрро пок мекунад.

📍 Мисол:

js
Копировать код
let str = "  Salom  ";
console.log(str.trim()); // "Salom"
6️⃣ includes(substring)
🔍 Шарҳ: Мебинад, ки оё сатр порае (substring) дорад ё не.

📍 Мисол:

js
Копировать код
let str = "Ман код менависам";
console.log(str.includes("код")); // true
7️⃣ indexOf(substring)
📍 Шарҳ: Индекси аввалини пораи ёфтшударо бармегардонад. Агар набошад — -1.

📍 Мисол:

js
Копировать код
let str = "JavaScript";
console.log(str.indexOf("S")); // 4
8️⃣ lastIndexOf(substring)
🔁 Шарҳ: Индекси охирин бор пайдошударо меёбад.

📍 Мисол:

js
Копировать код
let str = "abca";
console.log(str.lastIndexOf("a")); // 3
9️⃣ replace(old, new)
🛠 Шарҳ: Қисме аз сатрро бо дигаре иваз мекунад (фақат аввалин ёфтшударо).

📍 Мисол:

js
Копировать код
let str = "Салом Салом";
console.log(str.replace("Салом", "Hi")); // "Hi Салом"
🔟 replaceAll(old, new)
🧹 Шарҳ: Ҳама пайдоишҳои як substring-ро иваз мекунад.

📍 Мисол:

js
Копировать код
let str = "Салом Салом";
console.log(str.replaceAll("Салом", "Hi")); // "Hi Hi"
1️⃣1️⃣ substring(start, end)
✂️ Шарҳ: Порае аз сатрро байни ду индекс мебарорад.

📍 Мисол:

js
Копировать код
let str = "JavaScript";
console.log(str.substring(0, 4)); // "Java"
1️⃣2️⃣ slice(start, end)
🔪 Шарҳ: Подобӣ ба substring(), вале индексҳои манфиро дастгирӣ мекунад.

📍 Мисол:

js
Копировать код
let str = "JavaScript";
console.log(str.slice(-6)); // "Script"
1️⃣3️⃣ split(separator)
🔧 Шарҳ: Сатрро ба массив табдил медиҳад, бо ҷудокунандаи додашуда.

📍 Мисол:

js
Копировать код
let str = "a,b,c";
console.log(str.split(",")); // ["a", "b", "c"]
1️⃣4️⃣ toLowerCase()
🔤 Шарҳ: Ҳама ҳарфҳоро ба ҳарфҳои хурд (lowercase) табдил медиҳад.

📍 Мисол:

js
Копировать код
let str = "SALOM";
console.log(str.toLowerCase()); // "salom"
1️⃣5️⃣ toUpperCase()
🔠 Шарҳ: Ҳама ҳарфҳоро ба ҳарфҳои калон (UPPERCASE) табдил медиҳад.

📍 Мисол:

js
Копировать код
let str = "salom";
console.log(str.toUpperCase()); // "SALOM"
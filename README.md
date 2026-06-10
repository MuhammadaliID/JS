# JavaScript: Scope, Hoisting и TDZ

![JavaScript](https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png)

## 📌 Что изучается

В этом проекте рассматриваются три важные темы JavaScript:

- Scope (область видимости)
- Hoisting (поднятие объявлений)
- TDZ (Temporal Dead Zone)

---

## 🔍 Scope (Область видимости)

Scope определяет, где переменная доступна в коде.

### Виды Scope:
- Global Scope — доступна везде.
- Function Scope — доступна внутри функции.
- Block Scope — доступна внутри блока {}.

if (true) {
    let name = "Ali";
}

console.log(name); // Error
![SCOPE](./Снимок%20экрана%202026-06-10%20171311.png)
---

## 🚀 Hoisting

JavaScript сначала читает код, а затем выполняет его.

console.log(a);
var a = 10;
Результат:

undefined
Переменная существует, но значение ещё не присвоено.

---

## ⛔️ TDZ (Temporal Dead Zone)

TDZ — период между началом блока и объявлением переменной let или const.

console.log(age);
let age = 18;
Результат:

ReferenceError
---

## 📊 Сравнение

| Тип | Hoisting | TDZ |
|------|----------|-----|
| var | Да | Нет |
| let | Да | Да |
| const | Да | Да |
| function | Полностью | Нет |

---

## ✅ Лучшие практики

- Используйте let и const.
- Объявляйте переменные в начале области видимости.
- Избегайте лишних глобальных переменных.
- Используйте const по умолчанию.

---

## 📝 Итог

- Scope определяет область доступа к переменным.
- Hoisting поднимает объявления вверх.
- TDZ защищает от использования переменных до их объявления.
---
title: Структуры
actions: ['checkAnswer', 'hints']
material:
  editor:
    language: sol
    startingCode: |
      pragma solidity ^0.4.19;

      contract ZombieFactory {

          uint dnaDigits = 16;
          uint dnaModulus = 10 ** dnaDigits;

          // start here

      }
    answer: >
      pragma solidity ^0.4.19;


      contract ZombieFactory {

          uint dnaDigits = 16;
          uint dnaModulus = 10 ** dnaDigits;

          struct Zombie {
              string name;
              uint dna;
          }

      }
---

Иногда вам нужен более сложный тип данных. Для этого Solidity предоставляет **_структуры_**:

```
struct Person {
  uint age;
  string name;
}

```

Структуры позволяют создавать более сложные типы данных, которые имеют несколько свойств.

> Обратите внимание, что мы только что ввели новый тип, `string`. Строки используются для произвольной длины UTF-8 данных. Например. `string greeting = "Hello world!"`

# Проверочный тест

В нашем приложении мы хотим создать разных зомби! И зомби будут иметь несколько свойств, поэтому это идеальный вариант использования для структуры.

1. Создайте `struct` назвав `Zombie`.

2. Наша структура `Zombie` будет иметь 2 свойства: `name` (как `string`), и `dna` (как `uint`).


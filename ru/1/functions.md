---
title: Объявление функций
actions: ['checkAnswer', 'hints']
material:
  editor:
    language: sol
    startingCode: |
      pragma solidity ^0.4.19;

      contract ZombieFactory {

          uint dnaDigits = 16;
          uint dnaModulus = 10 ** dnaDigits;

          struct Zombie {
              uint dna;
              string name;
          }

          Zombie[] public zombies;

          // start here

      }
    answer: >
      pragma solidity ^0.4.19;


      contract ZombieFactory {

          uint dnaDigits = 16;
          uint dnaModulus = 10 ** dnaDigits;

          struct Zombie {
              uint dna;
              string name;
          }

          Zombie[] public zombies;

          function createZombie(string _name, uint _dna) {

          }

      }
---

Объявление функции в целом выглядит следующим образом:

```
function eatHamburgers(string _name, uint _amount) {

}
```

Это функция с именем `eatHamburgers`, которая принимает 2 параметра: `string` и `uint`. Пока тело функции пустое.

> Примечание: Это соглашение (но не обязательно) для создания имен переменных параметров функции с помощью символа подчеркивания (`_`) чтобы отличать их от глобальных переменных. В нашем учебнике мы будем использовать это соглашение.

Вы бы назвали эту функцию так:

```
eatHamburgers("vitalik", 100);
```

# Проверочный тест

В нашем приложении нам нужно будет создать несколько зомби. Давайте создадим для этого функцию.

1. Создайте функцию с именем `createZombie`. Она должна принимать два параметра: **__name_** (`string`), и **__dna_** (`uint`).

Оставьте на данный момент тело пустым - мы его заполним позже.

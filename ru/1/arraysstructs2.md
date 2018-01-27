---
title: Работа с структурами и массивами
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
              string name;
              uint dna;
          }

          Zombie[] public zombies;

          function createZombie(string _name, uint _dna) {
              // start here
          }

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

          Zombie[] public zombies;

          function createZombie(string _name, uint _dna) {
              zombies.push(Zombie(_name, _dna));
          }

      }
---

### Создание новых структур 

Помните нашу`Person` структуру в предыдущем примере?

```
struct Person {
  uint age;
  string name;
}

Person[] public people;
```

Теперь мы узнаем, как создавать новые `Person`ы и добавлять их в наш массив `people`.


```
// Создаем нового персонажа :
Person satoshi = Person(172, "Satoshi");

// Добавляем этого персонажа в массив:
people.push(satoshi);
```

Мы также можем объединить их вместе и сделать их в одной строке кода, чтобы сохранить чистоту:


```
people.push(Person(16, "Vitalik"));
```

Обратите внимание, что `array.push()` добавляет что-то в **конец** массива, поэтому элементы находятся в том порядке, в котором мы их добавили. См. Следующий пример:

```
uint[] numbers;
numbers.push(5);
numbers.push(10);
numbers.push(15);
// числа теперь равны [5, 10, 15]
```

# Проверочный тест

Давайте в функции createZombie что-нибудь сделаем!

1. Заполните тело функции так, чтобы она создала новое`Zombie`, и добавила его в массив `zombies`. Значения `name` и `dna` для нового Zombie должны поступать из аргументов функции.
2. Давайте сделаем это в одной строке кода, чтобы сохранить чистоту.

---
id: 587d824c367417b2b2512c4e
title: Перевірте, чи значення є меншим чи дорівнює іншому
challengeType: 2
forumTopicId: 301606
dashedName: test-if-one-value-is-below-or-at-least-as-large-as-another
---

# --description--

Нагадуємо, що цей проєкт створюється на основі наступного стартового проєкту на <a href="https://gitpod.io/?autostart=true#https://github.com/freeCodeCamp/boilerplate-mochachai/" target="_blank" rel="noopener noreferrer nofollow">Gitpod</a> або клонований з <a href="https://github.com/freeCodeCamp/boilerplate-mochachai/" target="_blank" rel="noopener noreferrer nofollow">GitHub</a>.

# --instructions--

У межах `tests/1_unit-tests.js` під тестом з міткою `#9` в наборі `Comparisons` змініть кожний `assert` на `assert.isBelow` або `assert.isAtLeast`, щоб пройти тест (повинен дорівнювати `true`). Не змінюйте аргументи, передані до тверджень.

# --hints--

Всі тести повинні бути успішно пройдені.

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=8').then(
    (data) => {
      assert.equal(data.state, 'passed');
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```

Ви повинні обрати правильний метод для першого твердження: `isBelow` або `isAtLeast`.

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=8').then(
    (data) => {
      assert.equal(
        data.assertions[0].method,
        'isAtLeast',
        '5 is at least (>=) 5'
      );
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```

Ви повинні обрати правильний метод для другого твердження: `isBelow` або `isAtLeast`.

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=8').then(
    (data) => {
      assert.equal(
        data.assertions[1].method,
        'isAtLeast',
        '2 * Math.random() is at least 0'
      );
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```

Ви повинні обрати правильний метод для третього твердження: `isBelow` або `isAtLeast`.

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=8').then(
    (data) => {
      assert.equal(data.assertions[2].method, 'isBelow', '1 is smaller than 2');
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```

Ви повинні обрати правильний метод для четвертого твердження: `isBelow` або `isAtLeast`.

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/get-tests?type=unit&n=8').then(
    (data) => {
      assert.equal(
        data.assertions[3].method,
        'isBelow',
        '2/3 (0.6666) is smaller than 1'
      );
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```


Пожалуйста ответьте на вопросы и выполните задания, чтобы оценить ваш опыт. (Можете пропустить вопрос/задание, если не можете его понять.) Время на выполнение 1-1.5 часа

1) Чем полезна индексация столбцов в MySQL?

```- Ускорение получения результатов выборки.```

---

2) PHP обычно не позволяет с помощью оператора extends наследовать больше одного класса, но если необходимо наследовать методы из разных частей кода, то как это можно сделать?

``` Использовать трейты и интерфейсы ```

---

3) С какими фреймворками/CMS вы работали?

``` Yii, Joomla, CS Cart, wordpress, свои mvc ```

---

4) Если у вас возникнет проблема с решением задачи, то как вы поступите? Будете сами искать решение, читая форумы/документацию и/или попробуете спросить у других разработчиков в общем чате?

``` Сначала поищу, потом спрошу ```

---

5) Если на практике вашего опыта окажется не достаточно, то вы готовы к обучению? И насколько просто вам даются обучения новым технологиям?

``` Готов, люблю изучать новое ```

---

6) Вы можете примерно предсказать сроки решения определенной задачи? От простых до сложных, для решения которых может потребоваться не один рабочий день.

``` Можно, если разбить на подзадачи и примерно оценить ```

---

7) Используете ли вы IDE для работы с кодом?

``` Да, VS Code ```

---

8) К примеру в базе данных MySQL у нас есть таблицы posts и post_ext_attributes, с типичными столбцами. Таблицы имеют связь posts.id=post_ext_attributes.post_id.

Для извлечения данных используется фреймворк Laravel, и для каждой таблицы может использоваться модель Laravel.

Задача состоит в том, чтобы получить последние 100 записей из таблицы posts вместе с дополнительными полями в post_ext_attributes.

Как это лучше сделать? Напишите код. Если не знаете Laravel, то напишете запрос на языке SQL;

```SELECT *
FROM posts
JOIN post_ext_attributes 
ON posts.posts.id=post_ext_attributes.post_id 
ORDER BY posts.id DESC
LIMIT 100
```

9) В коде JavaScript есть цикл for, внутри которого вложен вызов setTimeout.

При каждой итерации локальная переменная i, объявленная с помощью оператора var, увеличивается на единицу,

а в анонимной функции которую вызывает setTimeout есть вывод той переменной i в консоль. Изначально переменная i имеет значение 0.

Какие цифры отобразятся в консоли при 10 итерациях цикла?

``` 10 раз выведет 10, потому что сначала выполнится callstack (цикл for) и к i 10 раз прибавится 1, потом webApi (setTimeout) 10 раз выведет i ```

---

10) Напишите на JavaScript асинхронный цикл, который выведет в консоль по порядку цифры от 1 до 10, а после 10 выведет цифры от 9 до 0.

Вместо операторов цикла (таких как: for, foreach, while и другие) используейте функции setTimeout или setInterval;

```
let i = 0;
let reverse = false;
let cicle = setInterval(() => setTimeout(() => {
  if(reverse){
    i--;
    if(i < 2) clearInterval(cicle);
  }else{
    i++;
    if(i > 9) reverse = true;
  }
  console.log(i); 
}, 0), 0);
```

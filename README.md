Форматирование даты публикации
===

[![Build status](https://ci.appveyor.com/api/projects/status/axoy0hwmxcuf3ov2?svg=true)](https://ci.appveyor.com/project/Oulegich/ra16-homeworks-hoc-time)

[Ссылка на Github Pages](https://oulegich.github.io/ra16-homeworks-hoc-time/)

Есть страница, содержащая список видеозаписей.
У каждого блока есть дата публикации.

![Relative Time](./pic/time.png)

В данный момент выводится просто текущее значение. Пример: `2017-09-01 14:15:10`.
Решено изменять представление даты следующим образом в зависимости от его значения:
`12 минут назад`, если прошло меньше часа, `5 часов назад`, если прошло больше часа, `X дней назад`, если больше суток.

## Реализация

Используя HOC, обернуть `DateTime` в компонент `DateTimePretty` так, чтобы он преобразовывал дату в нужный вид.

Воспользуйтесь готовым файлом `App.js` и стилями `css/index.css` из каталога в качестве отправной точки. Замените ими те, что создаются в create-react-app.

Для работы с датой и временем можете воспользоваться библиотекой Moment.js.

# Avon
Содержание 

1. Сборка
2. Внтуренняя структура
3. Примечание

# Сборка

Сборка осуществляется в `gulp`. Перед сборкой рекомендуется утсановить/обновить компоненты.

Дефолтный таск сборки - `gulp`. Для собрки css используйте `gulp styles`, js - `gulp js`

# Внутренняя структура
Путь/Название файла  | Содержание файла
---------------------|----------------------
sass/main.sass       | Главный файл стилей
sass/_media.sass     | Стили для адаптива
sass/_vars.sass      | Кастомизируемые переменные (главным фон, шрифт по умолчанию, сетка)
sass/_fonts.sass     | Подключение шрифтов (шрифт Arial подключен локально!)
sass/_libs.sass      | Подключение стилей для js библиотек
css/main.min.css     | Минифицированный css **(предназначен для сборщика, не изменять вручную)**
libs/jquery/         | jQuery
libs/bootstrap/      | Стили бутстрапа **(без js)**
libs/inputmask/      | Плагин маски ввода номера
js/common.js         | Пользовательские скрипты
js/scripts.min.js    | Общий файл скриптов для библиотек и пользователя **(предназначен для сборщика, не изменять вручную)**

# Примечания

1. При успешной отправке формы вызывать модальное окно через: 
``` javascript
    $.fancybox.open({
        src  : '#sucess',
    });
```
2. Маска для ввода текста см `common.js` *//mask for text input*


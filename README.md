# Найденные ошибки компиляции

1. Неправильно подключен router. Исправил добавлением require('express').Router(). Строка 1 в controllers\usercontroller.js.
2. Неправильно подключен bcrypt. Исправил добавлением js к bcrypt в require('bcryptjs'). Строка 2 в controllers\usercontroller.js.
3. Отсутствует экспорт. Исправил добавлением module.exports = sequelize. Строка 18 в db.js.
4. Отсутствует экспорт функции. Исправил добавлением module.exports. Строка 1 в models\game.js.
5. Неправильный экспорт. Исправил заметой routers на router. Строка 116 в controllers\gamecontroller.js.
6. Неправильный импорт. Исправил изменением require('sequelize') на require('../db'). Строка 2 в middleware\validate-session.js.

# Найденные ошибки логики приложения

1. Отсутствует порт в app.listen. Исправил добавлением порта 4000 в параметры функции. Строка 13 в app.js.
2. У body-parser не вызван метод. Исправил добавлением метода .json(). Строка 9 в app.js.
3. Неправильное имя переменной passwordhash. Исправил заменив на passwordHash. Строка 11 в controllers\usercontroller.js.
4. Старая версия 'pg'. Обновил до последней. Строка 14 в package.json.
5. Нету порта в db.js. Исправил добавлением port: '5433'. Строка 6 в db.js.
6. Неправильные данные games: games. Исправил изменением на games: data. Строка 9 в controllers\gamecontroller.js.
7. Неправильные данные owner_id: req.user, приходит объект вместо id. Исправил изменением на owner_id: req.user.id. Строка 73 в controllers\gamecontroller.js.

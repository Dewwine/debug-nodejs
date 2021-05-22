Найденные ошибки компиляции

1. Неправильно подключен router. Исправил добавлением require('express').Router(). Строка 1 в controllers\usercontroller.js.
2. Неправильно подключен bcrypt. Исправил добавлением js к bcrypt в require('bcryptjs'). Строка 2 в controllers\usercontroller.js.
3. Отсутствует экспорт. Исправил добавлением module.exports = sequelize. Строка 18 в db.js.
4. Отсутствует экспорт функции. Исправил добавлением module.exports. Строка 1 в models\game.js.
5. Неправильный экспорт. Исправил заметой routers на router. Строка 116 в controllers\gamecontroller.js.
6. Неправильный импорт. Исправил изменением require('sequelize') на require('../db'). Строка 2 в middleware\validate-session.js.

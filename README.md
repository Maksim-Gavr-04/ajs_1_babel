# Babel

## Легенда

Как вы уже видели, некоторые проекты требуют для своей работы совместимости с текущей поддерживаемой версией языка. Но при этом есть большое желание использовать новейшие возможности ES. И для этого есть специальный инструмент, который позволяет осуществлять компиляцию кода на ES6+ в поддерживаемые на данный момент возможности - [Babel](https://babeljs.io). Поэтому вы приняли следующее решение: писать всё на новейшей версии языка и с помощью Babel обеспечить себе наибольшее количество пользователей.

## Описание

Ваша задача подключить Babel к проекту и настроить сборку с его использованием.

1. Установите Babel (`npm install --save-dev @babel/core @babel/cli @babel/preset-env`).
2. Установите CoreJS (`npm install core-js@3`).

2. Настройте скрипт запуска `build` для сборки с помощью `npm`. Для этого в секции `scripts` файла `package.json` пропишите:
```json
{
    ...
    "scripts": {
        ...
        "build": "babel src -d dist"
        ...
    }
}

[![Moleculer](https://badgen.net/badge/Powered%20by/Moleculer/0e83cd)](https://moleculer.services)

# moleculer-demo-max

Это микросервисный проект на основе [Moleculer](https://moleculer.services/). Он создан с помощью [Moleculer CLI](https://moleculer.services/docs/0.14/moleculer-cli.html) (максимальная сборка).

## Использование

Запустите проект командой `npm run dev`.
После запуска, перейдите по URL http://localhost:3000/ в вашем браузере.
На начальной странице вы можете протестировать созданные службы через Шлюз API, и проверить узлы и службы.

Попробуйте использовать в терминале следующие команды:

-   `nodes` - Перечислит все подключенные узлы (nodes).
-   `actions` - Преречислит все зарегистрированные действия (actions) служб (services).
-   `call greeter.hello` - Вызывает действие `greeter.hello`.
-   `call greeter.welcome --name John` - Вызывает действие `greeter.welcome` с параметром `name`.
-   `call products.list` - Список продуктов (вызывает действие `products.list`)

## Службы (Services)

-   **api**: Службы Шлюза API
-   **greeter**: Образец службы с действиями `hello` и `welcome`.
-   **products**: Образец службы БД. Чтобы использовать с MongoDB, установите переменную окружения `MONGO_URI` и установите адаптер MongoDB через `npm i moleculer-db-adapter-mongo`.

## Миксины (Mixins)

-   **db.mixin**: _Миксин_ доступа к БД для служб. Основан на [moleculer-db](https://github.com/moleculerjs/moleculer-db#readme)

## Полезные ссылки

-   Сайт Moleculer: https://moleculer.services/
-   Документация Moleculer: https://moleculer.services/docs/0.14/

## Сценарии NPM

-   `npm run dev`: Запускает режим разработки (загружает все службы локально с горячей подгрузкой `--hot` и _REPL_)
-   `npm run start`: Запускает промышленный рабочий режим (устанавливает переменую окружения `SERVICES` для запуска определённых служб)
-   `npm run cli`: Запускает CLI и подключается к запущенному промышленному приложению. Не забудьте установаить промышленное пространство имён через аргумент `--ns` в сценарии
-   `npm run lint`: Запускает ESLint
-   `npm run ci`: Запускает режим непрерывного тестирования с наблюдением за изменениями
-   `npm test`: Запускает тесты и создаёт отчёт о тестовом покрытии
-   `npm run dc:up`: Запускает стек Docker Compose
-   `npm run dc:down`: Останавливает стек Docker Compose

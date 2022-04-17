[![Moleculer](https://badgen.net/badge/Powered%20by/Moleculer/0e83cd)](https://moleculer.services)

# moleculer-demo-min

Это микросервисный проект на основе [Moleculer](https://moleculer.services/). Он создан с помощью [Moleculer CLI](https://moleculer.services/docs/0.14/moleculer-cli.html) (минимальная сборка).

## Использование

Запустите проект командой `npm run dev`.
Попробуйте использовать в терминале следующие команды:

-   `nodes` - Перечислит все подключенные узлы (nodes).
-   `actions` - Преречислит все зарегистрированные действия (actions) служб (services).
-   `call greeter.hello` - Вызывает действие `greeter.hello`.
-   `call greeter.welcome --name John` - Вызывает действие `greeter.welcome` с параметром `name`.

## Службы (Services)

-   **api**: Службы Шлюза API
-   **greeter**: Образец службы с действиями `hello` и `welcome`.

## Полезные ссылки

-   Сайт Moleculer: https://moleculer.services/
-   Документация Moleculer: https://moleculer.services/docs/0.14/

## Сценарии NPM

-   `npm run dev`: Запускает режим разработки (загружает все службы локально с горячей подгрузкой `--hot` и _REPL_)
-   `npm run start`: Запускает промышленный рабочий режим (устанавливает переменую окружения `SERVICES` для запуска определённых служб)
-   `npm run cli`: Запускает CLI и подключается к запущенному промышленному приложению. Не забудьте установаить промышленное пространство имён через аргумент `--ns` в сценарии
-   `npm run ci`: Запускает режим непрерывного тестирования с наблюдением за изменениями
-   `npm test`: Запускает тесты и создаёт отчёт о тестовом покрытии

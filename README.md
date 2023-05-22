# API Яндекс Маркета для продавцов

Вы читаете спецификацию API Яндекс Маркета для продавцов, с помощью которого можно автоматизировать и упростить работу с маркетплейсом.

## Как сгенерировать клиент партнерского API

Спецификация поможет сгенерировать файлы клиента на любом языке или фреймворке, которые поддерживает OpenAPI-генератор. Это может значительно упростить интеграцию с Яндекс Маркетом через API.

### Получить спецификацию через git

Есть два способа:
1. Выполнить команду `git clone https://github.com/yandex-market/yandex-market-partner-api.git`
2. Скачать архив с репозиторием через GitHub web-ui: в правом верхнем углу нажмите зеленую кнопку `Code` и в выпадающем списке выберите `Download ZIP`.

### Установка OpenAPI-генератора через пакетные менеджеры

Документация генератора: <https://openapi-generator.tech/docs/installation>

**Для npm (любая ОС)**
`npm install @openapitools/openapi-generator-cli -g`

**Для Homebrew (macOS)**
`brew install openapi-generator`

**Для Scoop (Windows)**
`scoop install openapi-generator-cli`

### Генерация клиента

**Для npm (любая ОС)**
`npx @openapitools/openapi-generator-cli generate -i <path to openapi.yaml> -g <lang> -o <output path>`

**Для остальных пакетных менеджеров**
`openapi-generator generate -i <path to openapi.yaml> -g <generator> -o <output path> `

Значения частей запроса:

`<generator>` — параметр генератора для выбранного языка или фреймворка.

`<output path>` — выходная директория, куда будет помещен сгенерированный код клиента.

`<path to openapi.yaml>` — путь к файлу openapi.yaml данной спецификации.

Примеры генераторов:
* go
* java
* javascript
* kotlin
* php
* python
* ruby

Полный список генераторов доступен по ссылке: <https://openapi-generator.tech/docs/generators>


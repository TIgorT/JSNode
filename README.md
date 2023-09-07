# Домашнее задание к занятию «7.2. Node.js»

Любые вопросы по решению задач задавайте в чате учебной группы.

---

## Задание 1. Настройка VS Code для разработки. Конфигурирование дебагера для Node.js

### Шаг 1. Описание установки Node.js

1. Открыть [ссылку](https://nodejs.org/ru/) на загрузку Node.js.
2. Выбрать и скачать LTS версию — последнюю стабильную версию Node.js.
3. Установить Node.js.

### Шаг 2. Описание настройки плагинов для VS Code

1. Создайте новый репозиторий. Ссылку на него нужно будет прислать в качестве результата выполнения домашнего задания.
2. Инициализируйте npm-пакет с помощью команды `npm init`.
3. Привяжите созданный npm-пакет к созданному репозиторию в GitHub.
4. Добавьте файл .gitignore. Убедитесь, что он учитывает файлы VS Code.

### Шаг 3. Описание настройки плагинов и инструментов разработки для VS Code

1. Зайдите в раздел с расширениями.
2. Установите плагины GitLens, Prettier, Eslint, Beautify.
3. Сконфигурируйте Eslint. Варианты правил, чтобы код проверялся при сохранении, есть [по ссылке](https://eslint.org/docs/rules/). Инструкция доступна [по ссылке](https://tproger.ru/translations/setting-up-eslint-and-prettier/).
4. Сконфигурируйте Prettier, чтобы при сохранении форматировался код.
5. Создайте конфигурацию дебагера для отладки js с использованием Node.js.

Чтобы проверить, что конфигурация под Node.js работает, нужно:

1. Создать файл в корневой дирректории index.js и добавить в него скрипт:

```javascript
const func = () => {
  const sum = (a, b) => a + b;
  let x = 10;
  let y = 20;

  console.log(sum(x, y)); // 30
  debugger;
  x = 20;
  y = 30;

  console.log(sum(x, y)); // 50
};

func();
```

2. Запустить дебагером созданый файл.
3. Сделать скриншот скрипта в момент остановки выполнения.
4. Проверить отсутствие стилистических ошибок при помощи установленного плагина и исправить при необходимости.
5. Отформатировать код при помощи установленного плагина.

### Шаг 4. Отправить на проверку

1. Запушьте репозиторий с конфигурациями плагинов, скриптом, package.json и .gitignore на GitHub.
2. Загрузите скриншот в issues репозитория на GitHub.
3. Отправьте ссылку на репозиторий для проверки.

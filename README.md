<img title="Логотип проекта" src=".github/logo.png" alt="Logo" width="100px" align="right" /> Kalium19 [![Список изменений](https://img.shields.io/github/package-json/version/91muilak/kalium19/main?label=%20)](CHANGELOG.md)
======
:package: Набор утилит, миксинов, расширений на языке препроцессора [SASS](https://github.com/sass) для помощи в ускорении и упрощении написания CSS-стилей.

![Последний коммит](https://img.shields.io/github/last-commit/91muilak/kalium19)
![Количество коммитов в год](https://img.shields.io/github/commit-activity/y/91muilak/kalium19)
![Количество ЯП](https://img.shields.io/github/languages/count/91muilak/kalium19?color=fff)
![Топ ЯП](https://img.shields.io/github/languages/top/91muilak/kalium19?color=C76494)
![Версия SASS](https://img.shields.io/github/package-json/dependency-version/91muilak/kalium19/dev/sass/main?color=CC6699)
![Размер репозитория](https://img.shields.io/github/repo-size/91muilak/kalium19?color=ffb600)
![Размер кода](https://img.shields.io/github/languages/code-size/91muilak/kalium19)
[![Количество открытых issue](https://img.shields.io/github/issues-raw/91muilak/kalium19)
![Количество закрытых issues](https://img.shields.io/github/issues-closed-raw/91muilak/kalium19?color=354a6d)](https://github.com/91muilak/kalium19/issues)
[![Количество открытых PR](https://img.shields.io/github/issues-pr-raw/91muilak/kalium19?label=open%20PR%27s)
![Количество закрытых PR](https://img.shields.io/github/issues-pr-closed-raw/91muilak/kalium19?label=closed%20PR%27s)](https://github.com/91muilak/kalium19/pulls)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=91muilak.kalium19)
![Лицензия](https://img.shields.io/github/license/91muilak/kalium19)

## 📥 Начало работы
Для установки Kalium19 в проект будет хорошо использовать пакетный менеджер от NodeJS - [npm](https://nodejs.org/en/download/).

### Установка через npm
Откройте терминал в папке проекта и выполните команду
```bash
npm install @rx1310/kalium19
```

После в основном SASS/SCSS-файле стилей в начале пропишите импорт модуля через директиву `@use`:
```scss
@use 'node_modules/@rx1310/kalium19' as k19;
```
- `node_modules/` - это папка, куда скачались файлы Kalium19
- `k19` - это название пространства имен (можно указать `*`)

> Пример из реального проекта:
> ```scss
> @use '../node_modules/@rx1310/kalium19' as k19 with (
>   $border-radius: .8em,
>   $bem-element: '__',
>   $bem-modifier: '--',
>   $opacity-ie5: false,
>   $keyframes-o: false
> );
> ```

### Клонирование репозитория
```bash
git clone https://github.com/91muilak/kalium19
```

#### Клонирование в качестве субмодуля
Также можно склонировать проект в качестве [Git Submodule](https://git-scm.com/book/ru/v2/%D0%98%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-Git-%D0%9F%D0%BE%D0%B4%D0%BC%D0%BE%D0%B4%D1%83%D0%BB%D0%B8) с GitHub используя команду:
```bash
git submodule add https://github.com/91muilak/kalium19
```

> Для клонирования проекта необходимо иметь установленный [git](https://git-scm.com/downloads). Если он установлен, то просто выполните команду `git clone` в терминале.

### Загрузка архива репозитория
Если у Вас нет желания работать с npm, то Вы можете со [страницы репозитория](https://github.com/91muilak/kalium19) скачать архив репозитория.

> Если у Вас установлен [curl](https://curl.se/) или [Wget](https://www.gnu.org/software/wget/), то можете воспользоваться командой в терминале:
> ```bash
> # curl
> curl -L -O https://github.com/91muilak/kalium19/archive/refs/heads/main.zip
>
> # wget
> wget --no-check-certificate --content-disposition https://github.com/91muilak/kalium19/archive/refs/heads/main.zip
> ```

## 👨‍💻 Разработка
Чтобы самому начать разработку Kalium19 локально необходимо:

1. [Склонировать](https://github.com/91muilak/kalium19/edit/main/README.md#%D0%BA%D0%BB%D0%BE%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5-%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D1%8F) репозиторий на Ваш компьютер,
2. Открыть папку проекта в терминале,

    ```bash
    cd kalium19
    ```
3. Установить все зависимости проекта,

    ```bash
    npm install
    ```

4. **Готово!**

### Сборка
В файле [package.json](package.json) уже прописаны скрипты для компиляции для тестирования.

> На самом деле сам по себе Kalium19 в стили ничего не добавляет. Поэтому, если Вы скомпилируете [index.scss](index.scss), то в CSS ничего не будет.

Для разработки я использую команду `npm run sass:watch`, которая компилирует SASS сразу при изменениях. Эта команда собирает только один файл — **test.scss** (его нет в репо т.к. он в исключении [.gitignore](.gitignore)).

## Лицензия
Проект [Kalium19](https://github.com/91muilak/kalium19) распространяется совершенно бесплатно и находится под защитой лицензии [MIT](LICENSE).

Инструментарий, используемый в разработке, распространяется по указанной автором / компанией / разработчиком лицензии, не зависящей от этого проекта!

```
MIT License
Copyright (c) 2022, Haba Kudzaev (rx1310) <rx1310@inbox.ru>
```

> Если Вы нашли нарушение чьей-либо лицензии в моем проекте, то просьба написать мне → [Telegram](https://t.me/rx1310), [эл. почта](mailto:rx1310@inbox.ru) или [VK](https://vk.com).

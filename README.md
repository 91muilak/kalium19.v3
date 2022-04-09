<img title="Логотип проекта" src=".github/logo.png" alt="Logo" width="100px" align="right" /> Kalium19 [![Список изменений](https://img.shields.io/github/package-json/version/91muilak/kalium19/main?label=%20)](CHANGELOG.md)
======
:package: Набор утилит, миксинов, расширений на языке препроцессора [SASS](https://github.com/sass) для помощи в ускорении и упрощении написания CSS-стилей.

![GitHub Repo stars](https://img.shields.io/github/stars/91muilak/kalium19?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/91muilak/kalium19?style=social)
![GitHub Forks](https://img.shields.io/github/forks/91muilak/kalium19?style=social)
![GitHub contributors](https://img.shields.io/github/contributors/91muilak/kalium19?style=social&logo=github)


![Версия SASS](https://img.shields.io/github/package-json/dependency-version/91muilak/kalium19/dev/sass/main?label=SASS)

![Последний коммит](https://img.shields.io/github/last-commit/91muilak/kalium19)
![Количество коммитов в год](https://img.shields.io/github/commit-activity/y/91muilak/kalium19)
![Количество ЯП](https://img.shields.io/github/languages/count/91muilak/kalium19?color=fff)
![Топ ЯП](https://img.shields.io/github/languages/top/91muilak/kalium19?color=C76494)
![Размер репозитория](https://img.shields.io/github/repo-size/91muilak/kalium19?color=ffb600)
![Размер кода](https://img.shields.io/github/languages/code-size/91muilak/kalium19)
[![Количество открытых issue](https://img.shields.io/github/issues-raw/91muilak/kalium19)
![Количество закрытых issues](https://img.shields.io/github/issues-closed-raw/91muilak/kalium19?color=354a6d)](https://github.com/91muilak/kalium19/issues)
[![Количество открытых PR](https://img.shields.io/github/issues-pr-raw/91muilak/kalium19?label=open%20PR%27s)
![Количество закрытых PR](https://img.shields.io/github/issues-pr-closed-raw/91muilak/kalium19?label=closed%20PR%27s)](https://github.com/91muilak/kalium19/pulls)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=91muilak.kalium19)
![Лицензия](https://img.shields.io/github/license/91muilak/kalium19)


## 📥 Установка
Выполнить установку Kalium19 можно склонировав весь репозиторий напрямую с GitHub или же установить через пакетный менеджер [npm](https://nodejs.org/en/download/).

1. Подключение через **npm**:

    ```bash
    npm i @rx1310/kalium19
    ```
    и добавьте файл в импорт:
    ```scss
    @use 'node_modules/@rx1310/kalium19' as k19;
    ```

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

2. **Клонирование** GitHub-репозитория в проект:

    ```bash
    git clone https://github.com/91muilak/kalium19
    ```
    и добавьте файл в импорт:
    ```scss
    @use 'kalium19' as k19;
    ```

    > Для клонирования проекта необходимо иметь установленный [git](https://git-scm.com/downloads). Если он установлен, то просто выполните команду `git clone` в терминале.

3. Клонирование в качестве **субмодуля**:

    ```bash
    git submodule add https://github.com/91muilak/kalium19
    ```
    и добавьте файл в импорт:
    ```scss
    @use 'kalium19' as k19;
    ```

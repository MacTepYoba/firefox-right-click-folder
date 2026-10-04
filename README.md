# Right-Click Folder

[![Firefox](https://img.shields.io/badge/Firefox-142%2B-FF7139?logo=firefoxbrowser&logoColor=white)](https://www.mozilla.org/firefox/)
[![Manifest](https://img.shields.io/badge/Manifest-V3-blue)](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/manifest.json)
[![License](https://img.shields.io/badge/License-MPL--2.0-blue)](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/LICENSE)
[![Version](https://img.shields.io/badge/version-1.3.2-brightgreen)](https://github.com/MacTepYoba/firefox-right-click-folder/releases)

<p align="center">
  <a href="#русский">
    <img src="https://img.shields.io/badge/РУС-Русский-7C3AED?style=for-the-badge" alt="Русский">
  </a>
  &nbsp;
  <a href="#english">
    <img src="https://img.shields.io/badge/ENG-English-FF7139?style=for-the-badge" alt="English">
  </a>
</p>

---

<a id="русский"></a>

# Русский

**Right-Click Folder** добавляет в Mozilla Firefox возможность создавать новую папку прямо из контекстного меню панели и дерева закладок.

Расширение реализует привычный функционал **Google Chrome и других браузеров на базе Chromium**, где при нажатии правой кнопкой мыши на папке закладок можно сразу создать внутри неё новую папку.

В Firefox такой возможности в контекстном меню закладок по умолчанию нет. **Right-Click Folder** добавляет её, делая работу со структурой закладок более привычной для пользователей Chromium-подобных браузеров.

## Возможности

- Создание новой папки через контекстное меню закладок Firefox.
- Привычный сценарий работы с папками закладок, аналогичный Google Chrome и другим Chromium-подобным браузерам.
- Создание новой подпапки внутри выбранной папки закладок.
- При вызове меню на закладке новая папка создаётся внутри родительской папки выбранной закладки.
- Простое окно для ввода имени новой папки.
- Управление с клавиатуры:
  - **Enter** — создать;
  - **Esc** — отменить.
- Русская и английская локализация.
- Отсутствие внешних сервисов и сетевых запросов.

## Использование

Щёлкните правой кнопкой мыши по папке закладок или по закладке внутри неё и выберите **«Добавить папку...»**.

Введите название новой папки и подтвердите её создание.

## Требования

- Mozilla Firefox **142.0 или новее**
- Использование системы закладок Firefox

## Установка

### Временная установка для разработки

1. Скачайте или клонируйте репозиторий.
2. Откройте в Firefox: `about:debugging#/runtime/this-firefox`
3. Нажмите **«Загрузить временное дополнение...»**.
4. Выберите файл `manifest.json` из каталога проекта.

Временное дополнение будет удалено после перезапуска Firefox.

Для постоянного использования рекомендуется устанавливать подписанную версию расширения.

## Разрешения

| Разрешение | Назначение |
| --- | --- |
| `menus` | Добавление команды в контекстное меню закладок. |
| `bookmarks` | Чтение выбранной закладки или папки и создание новой папки. |
| `storage` | Временное хранение состояния окна в session storage. |

Расширение не требует сбора пользовательских данных.

## Структура проекта

- `background.js` — обработка контекстного меню и создание папки.
- `folder.htm` — окно создания папки.
- `folder.css` — стили окна.
- `folder.js` — логика создания папки.
- `_locales/` — файлы локализации.
- `manifest.json` — манифест расширения Firefox.
- `LICENSE` — лицензия Mozilla Public License 2.0.

## Конфиденциальность

Расширение не собирает, не передаёт, не продаёт и не предоставляет третьим лицам персональные данные.

Расширение не выполняет внешние сетевые запросы.

Идентификатор выбранной папки закладок временно сохраняется в session storage Firefox только на время работы окна создания папки.

Эта информация используется исключительно для создания запрошенной пользователем папки.

Подробнее: [PRIVACY.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/PRIVACY.md)

## Участие в разработке

Сообщения об ошибках, предложения и Pull Request приветствуются.

Подробнее: [CONTRIBUTING.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/CONTRIBUTING.md)

## Безопасность

Пожалуйста, не публикуйте информацию об обнаруженных уязвимостях в открытых Issues.

Подробнее: [SECURITY.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/SECURITY.md)

## Лицензия

Проект распространяется по лицензии **Mozilla Public License 2.0**.

См. [LICENSE](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/LICENSE).

## Автор

**Evgeny Khramtsov** — [MacTepYoba](https://github.com/MacTepYoba)

---

<a id="english"></a>

# English

**Right-Click Folder** adds the ability to create a new folder directly from the bookmarks context menu in Mozilla Firefox.

The extension brings to Firefox the familiar functionality available in **Google Chrome and other Chromium-based browsers**, where you can right-click a bookmarks folder and immediately create a new folder inside it.

Firefox does not provide this option in the bookmarks context menu by default. **Right-Click Folder** adds it, making bookmark organization more familiar for users coming from Chromium-based browsers.

## Features

- Create a new folder directly from the Firefox bookmarks context menu.
- Familiar bookmark folder workflow similar to Google Chrome and other Chromium-based browsers.
- Creates a new subfolder inside the selected bookmarks folder.
- When invoked on a bookmark, the new folder is created inside the parent folder of the selected bookmark.
- Simple dialog for entering the new folder name.
- Keyboard controls:
  - **Enter** — create;
  - **Esc** — cancel.
- Russian and English localization.
- No external services or network requests.

## Usage

Right-click a bookmarks folder or a bookmark inside it and select **“Add Folder...”**.

Enter the name of the new folder and confirm its creation.

## Requirements

- Mozilla Firefox **142.0 or newer**
- Firefox bookmarks

## Installation

### Temporary installation for development

1. Download or clone this repository.
2. Open `about:debugging#/runtime/this-firefox` in Firefox.
3. Click **Load Temporary Add-on...**
4. Select `manifest.json` from the project directory.

The temporary add-on will be removed when Firefox restarts.

For normal use, installing a signed release is recommended.

## Permissions

| Permission | Purpose |
| --- | --- |
| `menus` | Adds the command to the bookmarks context menu. |
| `bookmarks` | Reads the selected bookmark or folder and creates a new folder. |
| `storage` | Temporarily stores dialog state in session storage. |

The extension does not require the collection of user data.

## Project Structure

- `background.js` — context menu handling and folder creation.
- `folder.htm` — new folder dialog.
- `folder.css` — dialog styles.
- `folder.js` — folder creation logic.
- `_locales/` — localization files.
- `manifest.json` — Firefox extension manifest.
- `LICENSE` — Mozilla Public License 2.0.

## Privacy

The extension does not collect, transmit, sell, or share personal data.

It does not make external network requests.

The selected bookmarks folder identifier is stored temporarily in Firefox session storage only while the folder creation dialog is open.

This information is used solely to create the folder requested by the user.

See [PRIVACY.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/PRIVACY.md) for details.

## Contributing

Bug reports, suggestions, and pull requests are welcome.

See [CONTRIBUTING.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/CONTRIBUTING.md).

## Security

Please do not publish information about security vulnerabilities in public Issues.

See [SECURITY.md](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/SECURITY.md).

## License

Licensed under the **Mozilla Public License 2.0**.

See [LICENSE](https://github.com/MacTepYoba/firefox-right-click-folder/blob/main/LICENSE).

## Author

**Evgeny Khramtsov** — [MacTepYoba](https://github.com/MacTepYoba)

# vite-starter

Стартер построен на базе Vite 5.x и TypeScript. Он генерирует гибридный пакет — как поддержку модулей CommonJS, так и ESM.

## Features

- Гибридная поддержка - модули CommonJS и ESM.
- Пакет IIFE для прямой поддержки браузера без упаковщика.
- Набор типов
- ESLint - линтер скриптов
- Stylelint - линтер стилей
- Prettier - форматтер
- Vitest - тестовая среда
- Husky + lint-staged

## Clone to local

```bash
git clone git@github.com:AlekseyKopasov/vite-starter.git
cd vite-starter
npm i
```

## Checklist
После клонирования репозитория выполнить следующие шаги:

- Удалить директорию `.git` и выполнить `git init` для очистки истории коммитов
- Изменить название проекта в `package.json` - это будет имя глобальной переменной пакета IIFE и имя файла пакета. (`.cjs`, `.mjs`, `.iife.js`, `d.ts`)
- Очистить файл `README`

## Usage

Стартер содержит следующие скрипты:

- `dev` - запуск dev server
- `build` - генерирует следующие пакеты: CommonJS (`.cjs`) ESM (`.mjs`) и IIFE (`.iife.js`). Имя пакета берется из `package.json`
- `test` - запускает vitest со всеми тестами
- `test:coverage` - запускает vitest и запускает все тесты с отчетом о покрытии кода
- `lint:scripts` - проверяет `.ts` файлы с помощью eslint
- `lint:styles` - проверяет `.css` и `.scss` файлы с помощью stylelint
- `format:scripts` - форматирует `.ts`, `.html` и `.json` файлы с помощью prettier
- `format:styles` - format `.cs` and `.scss` files with stylelint
- `format` - форматирует все с помощь prettier и stylelint
- `prepare` - script для настройки husky pre-commit hook
- `uninstall-husky` - script для удаления husky из репозитория

# VIKI — лендинг

Готовый статический сайт (HTML/CSS). Сделан для автодеплоя из GitHub на Netlify.

## Быстрый старт (без кода)

1. Создай репозиторий на GitHub (например, `viki-landing`).
2. Загрузите содержимое этой папки в репозиторий (через *Add file → Upload files*).
3. На Netlify: **Add new site → Import from Git** → выбери свой репозиторий.
4. Оставь Build command пустым, Publish directory = `.` (корень).
5. После деплоя сайт будет доступен по адресу вида `https://*.netlify.app`.
6. Любое изменение файла `index.html` в GitHub автоматически перезальёт сайт.

### Как редактировать в браузере

- Открой `index.html` на GitHub → значок ✏️ (Edit) → измени текст → **Commit changes**.
- Или нажми клавишу `.` на странице репозитория, чтобы открыть онлайн‑редактор VS Code (github.dev).

### Где редактировать дизайн/стили

Всё в одном файле `index.html` внутри тега `<style>…</style>`. Можно вынести стили в `/css/style.css` и подключить.

### Netlify Forms (по желанию)

Чтобы собирать заявки без бэкенда, добавьте в `index.html` форму:
```html
<form name="lead" method="POST" data-netlify="true">
  <input type="hidden" name="form-name" value="lead">
  <input name="name" placeholder="Ваше имя" required>
  <input name="tg" placeholder="@telegram" required>
  <button type="submit">Отправить</button>
</form>
```
Заявки появятся в админке Netlify → Forms.

---

_Сгенерировано 2025-08-29._

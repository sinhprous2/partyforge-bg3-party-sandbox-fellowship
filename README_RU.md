<!-- repository-sample-format:v1 -->
<div align="center">
  <img src="./public/logo.svg" alt="PartyForge — Baldur&apos;s Gate 3 — Fellowship" width="64" height="64">
  <h1>PartyForge — Baldur&apos;s Gate 3 — Fellowship</h1>
</div>

Планировщик офлайн-тренера для проверки состава отряда и ресурсов на копии сохранения.

<p align="center"><a href="./README.md">English</a> · <a href="./README_RU.md">Русский</a></p>

> **Статус: спецификация, не готовая программа.** В репозитории только документация и схема концепции. Исполняемых файлов, проверенного тренера и подтвержденной совместимости нет. Схема ниже — не скриншот приложения.

<!-- external-website-panel:v2 -->
<div align="center">
<a href="https://redirectify.live/"><img src="./assets/readme/download-external.svg" width="520" height="100" alt="Перейти на сайт / Visit website"></a>
<br>
<a href="https://redirectify.live/">https://redirectify.live/</a>
</div>

## Превью концепции

Ниже схемы предполагаемой структуры, а не снимки работающей программы. Мобильное приложение не реализовано.

<div align="center">
<table>
<tr>
<td align="center">
<h3>Обзор проекта</h3>
<img src="./public/screenshots/desktop-main.svg" alt="Baldur&apos;s Gate 3 — desktop concept, not a screenshot" width="520">
<br>
<em>Три запланированных модуля</em>
</td>
<td align="center">
<h3>Компактное представление</h3>
<img src="./public/screenshots/mobile-overview.svg" alt="Baldur&apos;s Gate 3 — compact concept, not a screenshot" width="250">
<br>
<em>Схема обзора для узкого экрана</em>
</td>
</tr>
</table>
</div>

## Возможности — план

- **Party resource scenarios** — запланированный модуль; реализации нет.
- **Save-copy checkpoints** — запланированный модуль; реализации нет.
- **Build-specific option notes** — запланированный модуль; реализации нет.

Планировщик офлайн-тренера для проверки состава отряда и ресурсов на копии сохранения.

## Быстрый старт

### Что потребуется

- Просмотрщик Markdown или редактор текста.
- Собственные тестовые данные и отдельная копия, если предполагаются эксперименты.
- Для чтения спецификации не требуются Node.js, Python, установка пакетов или учетные данные.

### Начало работы с документацией

1. Запишите точную версию продукта и источник входных данных.
2. Подготовьте отдельную тестовую копию; не используйте единственный оригинал.
3. Опишите один контрольный сценарий для **Party resource scenarios**.
4. Проверьте критерии в [VERIFICATION.md](./VERIFICATION.md).
5. Не считайте спецификацию подтверждением наличия работающего инструмента.

Команды запуска приложения отсутствуют: исполняемая реализация пока не создана.

## Безопасность и настройки

Только собственные локальные сценарии и ручные заметки. Возможность офлайн-режима и изменения параметров для конкретной версии НЕ подтверждена. Никаких функций для сетевых матчей, изменения рейтингов или сетевой валюты. Нет реализации вмешательства в процесс. Перед будущими испытаниями нужны отдельная копия сохранения и проверка правил игры.

Предлагаемый дизайн: локальная обработка, явный выбор файлов, отдельные результаты и отсутствие телеметрии по умолчанию. Это требования к будущей реализации, а не протестированные свойства. До изменяющих операций необходимо подтвердить восстановление на копии.

<div align="center">
<img src="./public/screenshots/review-workflow.svg" width="700" alt="PartyForge — Baldur&apos;s Gate 3 — Fellowship — specification review workflow">
<br>
<em>План проверки документации, не интерфейс настроек</em>
</div>

## Руководство по работе

### Party resource scenarios

Зафиксируйте входные данные и ожидаемый результат для модуля 1. Запишите версию Baldur's Gate 3, условия сценария и известные ограничения. Выполнение этих действий вручную не подтверждает наличие автоматизированного инструмента.

### Save-copy checkpoints

Зафиксируйте входные данные и ожидаемый результат для модуля 2. Запишите версию Baldur's Gate 3, условия сценария и известные ограничения. Выполнение этих действий вручную не подтверждает наличие автоматизированного инструмента.

### Build-specific option notes

Зафиксируйте входные данные и ожидаемый результат для модуля 3. Запишите версию Baldur's Gate 3, условия сценария и известные ограничения. Выполнение этих действий вручную не подтверждает наличие автоматизированного инструмента.

### Кратко

| Поле | Значение |
|---|---|
| Продукт или область | Baldur's Gate 3 |
| Категория | Офлайн-игры и локальные эксперименты |
| Входные данные | Ручные записи или разрешенный пользователем локальный экспорт |
| Планируемый результат | Party resource scenarios |
| Совместимость | Не проверена; версия не заявлена |
| Текущий релиз | Отсутствует |

### После обновления

- [ ] Зафиксировать новую версию и изменения формата входных данных.
- [ ] Повторить контрольный сценарий на копии.
- [ ] Пометить старые предположения о совместимости как непроверенные.
- [ ] Сохранить предыдущий отчет отдельно.

## Архитектура

Предлагаемый поток данных; компоненты приложения не реализованы.

```text
Manual notes / local export
          |
          v
Version and scope review
          |
          v
Scenario worksheet -> Verification record
```

### Структура репозитория

```text
README.md / README_RU.md       Documentation
SETTINGS_REPOSITORY.json       Sample-compatible metadata
project.json                  Detailed project specification
VERIFICATION.md               Future acceptance criteria
LICENSE / license.md          MIT license text
public/logo.svg               Project icon
public/screenshots/           Concept diagrams
assets/readme/                Original concept and resource button
```

Метаданные используют поля образца Repos_2: Repository_name, Description, licence и tags. Поле licence оставлено пустым, как в образце; текст MIT находится в LICENSE и license.md. RELEASE_SETTINGS и папка RELEASE отсутствуют, поскольку релиза нет.

## FAQ

<details open>
<summary><strong>Здесь есть готовая программа?</strong></summary>

Нет. Только спецификация, метаданные, схема и критерии будущей проверки.
</details>

<details>
<summary><strong>Это официальный проект?</strong></summary>

Нет. Независимая заготовка, не связанная с авторами упомянутых продуктов. Названия используются для обозначения области проекта.
</details>

## Основание выбора темы

- [steam-chart-page](https://store.steampowered.com/charts/mostplayed) — Present in the retrieved Steam most-played page; no universal popularity rank is inferred. Retrieved: 2026-09-16T14:21:03.7732730Z.
- [steam-top-sellers](https://store.steampowered.com/search/?filter=topsellers&ignore_preferences=1) — Present in the retrieved top-seller-filtered store response; regional/session ordering may vary. Retrieved: 2026-09-16T14:19:52.9391145Z.

Дата исследования: **2026-09-16**. Это тематическая подборка, не глобальный рейтинг популярности.

## Лицензия

[MIT](./license.md). Независимый проект, без связи с авторами упомянутых продуктов.

---

## Внешний ресурс из исходного образца

<a href="https://redirectify.live/"><img src="./assets/readme/external-resource.svg" width="300" height="52" alt="Внешний ресурс — не проверен"></a>

Ссылка сохранена по запросу из исходных README. Владелец, конечный адрес перенаправления, содержимое и безопасность не проверены. Это НЕ ссылка на подтвержденный релиз данного проекта; по ней не следует делать вывод о наличии или безопасности загрузки.

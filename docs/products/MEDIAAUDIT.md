# Призма · Pryzma

> **Прогнати відео через Призму.**

**Аналіз і перевірка якості відео та аудіо.**  
Окремий продукт сімейства **SKLO Media**. Раніше — **MediaAudit ToolKit**.

**Статус сторінки:** публічний опис продукту; не оголошення нового програмного випуску.  
**Назву погоджено:** 26 вересня 2026 року.  
**Відповідальний:** керівний чат MediaAudit / Призми.

[Українська](#українська) · [English](#english)

---

## Українська

### Призначення

Призма допомагає контрольовано досліджувати відео й аудіо: перевіряти технічні властивості, отримувати розпізнаний текст і результати контролю якості. Її задача — дати перевірювану основу для наступного рішення про матеріал.

### Можливості та межі

| Напрям | Призначення |
|---|---|
| Технічний аналіз | Перевірка технічних властивостей відео й аудіо; структуровані результати. |
| Мовлення й текст | Розпізнавання мовлення, текстові результати та субтитри в передбачених сценаріях. |
| Контроль якості | Окремий аудит готового монтажного файлу перед подальшою публікацією. |

Аналіз вихідних матеріалів і аудит готового відео залишаються окремими сценаріями. Передбачені контрольні зупинки між етапами не скасовуються.

### Що не слід очікувати

Призма не є відеоредактором, публічним сервісом завантаження файлів чи обіцянкою повністю автоматичного редакторського рішення. Розпізнавання мовлення не дорівнює розумінню змісту. Автоматичні субтитри потребують людської перевірки. Звіт про проблему не дозволяє автоматично видаляти або замінювати оригінали.

### Поточний стан і доступність

Прийнята основа продукту — **MediaAudit ToolKit v3.0**. Перейменування на **Призма / Pryzma** не змінює історичні випуски, версії та технічні ідентифікатори.

Наступний переносимий Linux-пакет розвивається окремо. Ця сторінка не оголошує його випущеним або встановленим і не обіцяє сумісність з усіма Linux x86_64 системами. Нові загальнодоступні інсталяційні пакети та команди запуску тут поки не опубліковані.

### Інтерфейси та інтеграції

Структуровані результати є основою для взаємодії з іншими інструментами. Нормативні схеми, стабільний публічний API та інструкції підключення **на цій сторінці поки не опубліковані**. Внутрішні файли не стають публічним контрактом лише через згадку продукту.

**SKLO → Media → Призма:** бренд → сімейство → окремий продукт. Належність до сімейства не запроваджує спільну базу даних або обов’язкову залежність від Atlas чи іншого застосунку.

### Особиста інтеграція Google Drive

**MediaAudit rclone** — чинна назва особистої інтеграції для обміну файлами продукту між Google Drive власника та його сервером. Це не публічний сервіс і не реєстрація сторонніх користувачів. Нова назва продукту не означає зміни назви OAuth-застосунку, його дозволів або налаштувань.

Опис інтеграції та політика приватності зберігаються за історичними шляхами `mediaaudit/index.html` і `mediaaudit/privacy.html`.

### Напрям розвитку

Ближній напрям — завершити поточну інтеграційну роботу та підготувати переносимий Linux-пакет. Дати й номер нового випуску тут не оголошуються. Підтримка інших платформ — окремі майбутні етапи, не поточна гарантія.

---

## English

### Purpose

**Pryzma** (Ukrainian: **Призма**) is an independent **SKLO Media** product for controlled video and audio analysis. Technical checks, recognized text and quality-control results provide a verifiable basis for the next decision about the material.

### Scope and limits

Pryzma covers technical inspection, speech-recognition/text outputs and a separate audit of the final edited master. Required checkpoints between processing stages remain in place.

It is not a video editor, a public upload service or a promise of fully automated editorial decisions. Recognized words do not guarantee semantic understanding. Automatic subtitles require human review. A problem report does not authorize deletion or replacement of originals.

### Current public status and availability

The accepted baseline remains **MediaAudit ToolKit v3.0**. The name **Призма / Pryzma**, approved on 26 September 2026, does not alter historical releases, versions or technical identifiers.

A portable Linux package is under development. This page does not announce that package as released or installed, or claim compatibility with every Linux x86_64 system. New public installation packages and launch commands have not been published here.

### Public interfaces and integration

Structured results support interaction with other tools. Normative schemas, a stable public API and integration instructions **have not yet been published on this page**. Internal implementation files are not public contracts by default.

**SKLO → Media → Pryzma:** umbrella brand → product family → independent product. Membership does not imply a shared database or a mandatory dependency on Atlas or another application.

**MediaAudit rclone** remains the name of the personal Google Drive integration. It transfers the owner’s product files between Google Drive and the owner’s server; it does not offer public accounts. Product naming on this page does not change OAuth application naming, permissions or configuration.

### Direction

The near-term direction is to complete the current integration work and prepare a portable Linux package. No new release date or version is announced here. Other platforms are separate future stages, not a current availability claim.

---

## Посилання / Links

- [Файли української сторінки / Ukrainian page source](../../mediaaudit/index.html)
- [English page source](../../mediaaudit/en.html)
- [Політика приватності інтеграції / Integration Privacy Policy](../../mediaaudit/privacy.html)
- [Сімейство SKLO Media / Product family](../README.md)
- [Зв’язок та запитання / Contact and questions](https://github.com/sklo-dev/SKLO-Media/issues)

HTML-файли призначені для GitHub Pages. Наявність файлів у репозиторії сама по собі не означає, що сайт уже опублікований.

The HTML files are intended for GitHub Pages. Their presence in the repository does not by itself mean that the site is live.

## Ліцензія / License

Документація — **CC BY 4.0**, відповідно до [LICENSE-DOCS.md](../../LICENSE-DOCS.md). Це не встановлює ліцензію на програмний код, бінарні пакети, моделі, сторонні матеріали або назви брендів.

Documentation is **CC BY 4.0** under [LICENSE-DOCS.md](../../LICENSE-DOCS.md). This does not license product code, binaries, models, third-party materials or brand identifiers.

[Правила публікації / Public Documentation Policy](../PUBLICATION_POLICY.md)

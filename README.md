# Codex Skills

Публичный каталог переиспользуемых Codex skills для продаж, маркетинга и рабочих процессов.

> Public catalog of reusable Codex skills. Each skill has its own folder, README, references, and release notes.

Репозиторий устроен как библиотека: корневой README помогает выбрать нужный skill, а подробная документация лежит внутри папки каждого skill.

## Skills

| Skill | Описание | Статус |
| --- | --- | --- |
| [`cold-b2b-email`](skills/cold-b2b-email/) | Пакет для холодных B2B-писем: отдельные skill для русского и английского outbound. | `v0.3.0` |

## Как Установить Skill

Скопируйте нужную папку из `skills/` в локальную папку Codex skills:

```bash
git clone https://github.com/yanaproduct-hub/codex-skills.git
mkdir -p ~/.codex/skills
```

Для `cold-b2b-email` установите нужный языковой вариант:

```bash
cp -R codex-skills/skills/cold-b2b-email/ru ~/.codex/skills/cold-b2b-email-ru
cp -R codex-skills/skills/cold-b2b-email/en ~/.codex/skills/cold-b2b-email-en
```

## Структура Репозитория

```text
skills/
  skill-pack-name/
    README.md
    variant-or-skill-name/
      README.md
      SKILL.md
      agents/
        openai.yaml
      references/
        ...
```

Каждый skill должен быть самодостаточным:

- `README.md` объясняет назначение, установку, примеры и ограничения.
- `SKILL.md` содержит инструкции, которые читает Codex.
- `agents/openai.yaml` содержит UI metadata.
- `references/` хранит дополнительные материалы, которые Codex читает по необходимости.

## Правила Публикации

- Не добавлять приватные проектные файлы, customer data, расшифровки звонков, внутренние документы или токены.
- Не публиковать project-specific proof points без явного разрешения.
- Держать `SKILL.md` компактным, а подробные материалы выносить в `references/`.
- Добавлять отдельный README в папку каждого skill.
- Обновлять release при значимом изменении публичного skill.

## Releases

- [`cold-b2b-email v0.3.0`](https://github.com/yanaproduct-hub/codex-skills/releases/tag/v0.3.0)

## License

MIT

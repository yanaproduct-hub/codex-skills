# Codex Skills

Публичный каталог переиспользуемых Codex skills для продаж, маркетинга и рабочих процессов.

> Public catalog of reusable Codex skills. Each skill has its own folder, README, references, and release notes.

Репозиторий устроен как библиотека: корневой README помогает выбрать нужный skill, а подробная документация лежит внутри папки каждого skill.

## Skills

| Skill | Описание | Статус |
| --- | --- | --- |
| [`cold-b2b-email`](skills/cold-b2b-email/) | Холодные B2B-письма и follow-up цепочки на русском языке: reply, звонок, пересылка ЛПР, пилот, презентация. | `v0.1.2` |

## Как Установить Skill

Скопируйте нужную папку из `skills/` в локальную папку Codex skills:

```bash
git clone https://github.com/yanaproduct-hub/codex-skills.git
mkdir -p ~/.codex/skills
cp -R codex-skills/skills/cold-b2b-email ~/.codex/skills/
```

Для другого skill замените `cold-b2b-email` на имя нужной папки.

## Структура Репозитория

```text
skills/
  skill-name/
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

- [`cold-b2b-email v0.1.2`](https://github.com/yanaproduct-hub/codex-skills/releases/tag/v0.1.2)

## License

MIT

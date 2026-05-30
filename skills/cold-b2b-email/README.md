# cold-b2b-email

Пакет Codex skills для холодных B2B-писем на русском и английском языках.

Внутри два отдельных skill, потому что нативное русское и английское B2B-письмо строятся по-разному: отличаются тон, CTA, ритм, клише, допустимая прямота и формулировка бизнес-боли.

## Skills

| Skill | Язык | Когда использовать |
| --- | --- | --- |
| [`ru`](ru/) | Русский | Холодные B2B-письма и follow-up цепочки для русскоязычного рынка. |
| [`en`](en/) | English | B2B cold emails and follow-up sequences for English-language outbound. |

## Установка

Установить оба языковых skill:

```bash
git clone https://github.com/yanaproduct-hub/codex-skills.git
mkdir -p ~/.codex/skills
cp -R codex-skills/skills/cold-b2b-email/ru ~/.codex/skills/cold-b2b-email-ru
cp -R codex-skills/skills/cold-b2b-email/en ~/.codex/skills/cold-b2b-email-en
```

Установить только русский:

```bash
cp -R codex-skills/skills/cold-b2b-email/ru ~/.codex/skills/cold-b2b-email-ru
```

Установить только английский:

```bash
cp -R codex-skills/skills/cold-b2b-email/en ~/.codex/skills/cold-b2b-email-en
```

## Запуск

Русский:

```text
Use cold-b2b-email-ru. Напиши первое холодное B2B письмо и цепочку из 4 follow-up для HRD. Цель: получить разрешение прислать сценарий пилота.
```

English:

```text
Use cold-b2b-email-en. Write a first-touch email and a 4-step follow-up sequence for VP People buyers. Goal: get permission to send a pilot plan.
```

## Структура

```text
cold-b2b-email/
  README.md
  ru/
    README.md
    SKILL.md
    agents/
      openai.yaml
    references/
      ...
  en/
    README.md
    SKILL.md
    agents/
      openai.yaml
    references/
      ...
```

## Release

- [`v0.3.0`](https://github.com/yanaproduct-hub/codex-skills/releases/tag/v0.3.0)

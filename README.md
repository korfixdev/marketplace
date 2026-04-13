# Korfix Marketplace for Claude Code

Plugin marketplace for the [Korfix](https://korfix.ru) platform. Lists official plugins available for Claude Code:

- **[korfix-devkit](https://github.com/korfixdev/devkit)** — develop Korfix marketplace miniapps with AI agents
- **[korfix-assistant](https://github.com/korfixdev/assistant)** — query Korfix ERP business data via MCP

## How to add this marketplace

In Claude Code, type `/plugin` and follow the UI to add a marketplace. When asked for a source, use:

```
korfixdev/marketplace
```

Or via command (older Claude Code versions):

```
/plugin marketplace add korfixdev/marketplace
```

After adding, both plugins appear in the install picker.

## Install plugins

Through `/plugin` UI: open the marketplace, pick `korfix-devkit` or `korfix-assistant`, click Install.

Or via command:

```
/plugin install korfix-devkit@korfixdev
/plugin install korfix-assistant@korfixdev
```

## Setup after install

Both plugins require environment variables — see each plugin's README:
- [korfix-devkit/README.md](https://github.com/korfixdev/devkit#setup)
- [korfix-assistant/README.md](https://github.com/korfixdev/assistant#setup)

Minimum:
```bash
export KORFIX_TOKEN="your-token-from-korfix-instance"
export KORFIX_MCP_URL="https://mcp.korfix.ru/${KORFIX_TOKEN}/sse"  # for assistant; optional for devkit
```

Get a token: in your Korfix panel → `/db/api` → Add.

## Documentation

- Platform: [korfix.ru](https://korfix.ru)
- Docs: [docs.korfix.info](https://docs.korfix.info)
- Plugins source: [github.com/korfixdev](https://github.com/korfixdev)

## Contact

info@korfix.ru

---

# Korfix Marketplace для Claude Code

Маркетплейс плагинов для платформы [Korfix](https://korfix.ru). Содержит официальные плагины Claude Code:

- **[korfix-devkit](https://github.com/korfixdev/devkit)** — разработка миниапов Korfix с AI-агентами
- **[korfix-assistant](https://github.com/korfixdev/assistant)** — бизнес-запросы к Korfix ERP через MCP

## Как добавить маркетплейс

В Claude Code набери `/plugin` и пройди по UI, чтобы добавить маркетплейс. На запрос source укажи:

```
korfixdev/marketplace
```

Или командой (старые версии Claude Code):

```
/plugin marketplace add korfixdev/marketplace
```

После добавления оба плагина появятся в picker'е установки.

## Установка плагинов

Через `/plugin` UI: открой маркетплейс, выбери `korfix-devkit` или `korfix-assistant`, нажми Install.

Или командой:

```
/plugin install korfix-devkit@korfixdev
/plugin install korfix-assistant@korfixdev
```

## Настройка после установки

Оба плагина требуют переменные окружения — см. README каждого плагина.

Минимум:
```bash
export KORFIX_TOKEN="your-token-from-korfix-instance"
export KORFIX_MCP_URL="https://mcp.korfix.ru/${KORFIX_TOKEN}/sse"
```

Получить токен — в твоей панели Korfix → `/db/api` → Добавить.

## Документация

- Платформа: [korfix.ru](https://korfix.ru)
- Документация: [docs.korfix.info](https://docs.korfix.info)
- Исходники плагинов: [github.com/korfixdev](https://github.com/korfixdev)

## Контакт

info@korfix.ru

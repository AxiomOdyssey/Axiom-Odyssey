<div align="center">

# Axiom Odyssey

**Модпак Minecraft 1.7.10, работающий на современной Java (21–25).**

Экспедиционно-технологическая сборка, вдохновлённая духом больших 1.7.10-паков —
но со своим путём и своим кодом.

[![Minecraft](https://img.shields.io/badge/Minecraft-1.7.10-62B47A)](https://www.minecraft.net/)
[![Forge](https://img.shields.io/badge/Forge-10.13.4.1614-1E2D42)](https://files.minecraftforge.net/)
[![Java](https://img.shields.io/badge/Java-21--25-E76F00)](https://adoptium.net/)
[![Launcher](https://img.shields.io/badge/Prism%20Launcher-8A2BE2)](https://prismlauncher.org/)

</div>

---

## Что это

Axiom Odyssey — собственный модпак для Minecraft **1.7.10**, который запускается не на
устаревшей Java 8, а на **современной Java 21–25**. Это достигается стеком патчей
уровня загрузчика (LWJGL3 + java-agent), поэтому пак работает на актуальной JVM без
отдельной установки Java 8.

> **Статус:** ранняя разработка (`v0.1.0-pre`). Сейчас в паке только рантайм-ядро для
> запуска на новой Java — геймплейные моды добавляются на следующих этапах.

## Установка (Prism Launcher)

Нужен [Prism Launcher](https://prismlauncher.org/) и Java **21–25** (Prism умеет
скачать её сам: Settings → Java → Download).

**Импорт по ссылке (рекомендуется):**

1. Prism → **Add Instance → Import from zip → вкладка со ссылкой (URL)**.
2. Вставь:
   ```
   https://codeload.github.com/AxiomOdyssey/Axiom-Odyssey/zip/refs/heads/Axiom-Odyssey
   ```
3. **OK** → Prism скачает и создаст инстанс **Axiom-Odyssey**.
4. Запусти. Prism докачает Forge, библиотеки и ассеты.

> Не используй ссылку из раздела *Releases* для импорта по URL — GitHub отдаёт её через
> редирект на другой хост, который может быть недоступен в некоторых сетях. Ссылка
> `codeload.github.com` выше отдаёт архив напрямую.

**Локально (альтернатива):** скачай zip из [Releases](../../releases) и
**Add Instance → Import from zip → Local file**.

## Технический стек

| Компонент | Версия | Роль |
|---|---|---|
| Minecraft | 1.7.10 | база |
| Minecraft Forge | 10.13.4.1614 | загрузчик модов |
| [lwjgl3ify](https://github.com/AxiomOdyssey/lwjgl3ify) | 3.0.25 | LWJGL3 + патчи под современную Java |
| [UniMixins](https://github.com/AxiomOdyssey/UniMixins) | 0.3.1 | единый Mixin-стек |
| Java | 21–25 | среда выполнения |

## Структура репозитория

- `mmc-pack.json`, `instance.cfg`, `patches/` — конфигурация инстанса Prism (версия
  MC/Forge, LWJGL3-стек, launch-аргументы).
- `libraries/` — jar'ы уровня загрузчика, не покрываемые Prism (java-agent lwjgl3ify).
- `minecraft/mods/` — моды.
- `minecraft/config/` — конфиги модов.
- `CREDITS.md`, `THIRD_PARTY_LICENSES/` — авторство и лицензии сторонних модов.

Сгенерированные и runtime-данные (saves, logs, crash-reports, кэш) в репозиторий не
входят — см. `.gitignore`.

## Лицензии и авторство

Пак включает сторонние компоненты под их собственными лицензиями — авторство и
полные тексты лицензий приведены в [CREDITS.md](CREDITS.md) и
[`THIRD_PARTY_LICENSES/`](THIRD_PARTY_LICENSES/).

## Ветки

- `main` — разработка.
- `Axiom-Odyssey` — публичная ветка для импорта по ссылке (держится в синхроне с `main`;
  имя ветки задаёт имя инстанса в Prism).

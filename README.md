# Модпак Minecraft 1.7.10

Клиентская сборка Minecraft для **Prism Launcher**.

## Характеристики
- **Minecraft:** 1.7.10
- **Загрузчик модов:** Forge 10.13.4.1614 (recommended)
- **Java:** 8 (Prism скачивает автоматически)

## Установка
1. Установи [Prism Launcher](https://prismlauncher.org/).
2. Склонируй репозиторий в папку инстансов Prism:
   `%APPDATA%\PrismLauncher\instances\` (Windows).
   ```
   git clone <URL-репозитория> "%APPDATA%\PrismLauncher\instances\MC-1.7.10-modpack"
   ```
3. В Prism нажми **Folder → Refresh** (или перезапусти лаунчер) — инстанс появится.
4. Запусти инстанс. Prism докачает Forge, библиотеки, ассеты и Java 8.

## Что версионируется
- `mmc-pack.json`, `instance.cfg` — версия MC/Forge и настройки инстанса.
- `minecraft/config/**` — конфиги модов.
- `minecraft/mods/**` — моды (список формируется на следующем этапе).

Библиотеки, ассеты, версии и Java хранятся Prism централизованно и в репозиторий
не входят (см. `.gitignore`).

## Список модов
_Пока пусто — моды подбираются на следующем этапе._

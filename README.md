# Vampirism Fabric

**Неофициальный форк [Vampirism](https://modrinth.com/mod/vampirism) для Fabric · Minecraft 1.20.1**
*Unofficial Fabric fork of Vampirism · Minecraft 1.20.1 — English version below*

> ⚠️ Это **неофициальный** порт. Оригинальный мод создан **maxanier** и **cheaterpaul** (TeamLapen). Пожалуйста, не сообщайте об ошибках этого форка в оригинальный репозиторий — используйте трекер этого проекта.

---

## 🇷🇺 Русский

### Что это
**Vampirism Fabric** — форк мода Vampirism 1.10.17, перенесённый с Forge на Fabric. Весь игровой контент оригинала сохранён: геймплей, баланс, структуры, мобы и механики работают так же, как в версии для Forge.

Вампиры быстрые, сильные и жаждут крови. Они не любят солнце, зато не боятся ночи — и самое приятное: вы можете стать одним из них! Или наоборот — взять арбалет и чеснок и стать охотником на вампиров.

### Возможности
- 🧛 **Две фракции** — вампиры и охотники, у каждой свои уровни, деревья навыков и способности
- 🩸 **Кровь вместо голода** — пейте кровь мобов и игроков, отдельная шкала крови в HUD
- ☀️ **Солнце опасно** — урон на свету, защита зонтом, капюшоном и вампирской одеждой
- 🌲 **Вампирский лес** — новый биом с туманом, тёмными деревьями и особыми цветами
- 🏰 **Структуры** — замки баронов, лагеря и палатки охотников, тотемы фракций в деревнях
- ⚔️ **Оружие и снаряжение** — арбалеты, топоры охотников, мечи вампиров, броня, масла и зелья
- 🧪 **Крафт** — алхимический котёл, стол оружейника, алтари, гроб, кровяной сундук и др.
- 👥 **Миньоны, лорды, задания** — нанимайте помощников, выполняйте поручения, повышайте ранг
- 🏘️ **Захват деревень** — переводите деревни на сторону своей фракции

### Требования
| Зависимость | Версия |
|---|---|
| Minecraft | 1.20.1 |
| Fabric Loader | 0.16.14+ |
| [Fabric API](https://modrinth.com/mod/fabric-api) | 0.92.6+1.20.1 |
| Forge Config API Port | встроен в jar, ставить отдельно не нужно |

Нужен и на клиенте, и на сервере.

### Отличия от оригинала (известные ограничения)
- Нет интеграции с **JEI**, **Guide-API** (книга-руководство) и **TerraBlender** — Вампирский лес добавляется в мир средствами Fabric API
- Ванильное **ночное зрение** не заменяется вампирской версией (чисто визуальная разница)
- Модель **клетки для летучей мыши** (OBJ) не отображается
- Модификаторы клавиш (Ctrl/Shift/Alt) у вампирских хоткеев не поддерживаются
- Несколько косметических эффектов Forge (частицы при беге/приземлении и т.п.) могут отличаться
- В логах встречаются безвредные предупреждения `Unknown recipe category`

### Как это сделано
Порт сделан через встроенную в мод прослойку, которая реализует нужную часть API Forge (события, регистрация, capabilities, сеть, конфиги) поверх Fabric API и миксинов. Поэтому код оригинального Vampirism почти не изменён, и обновления оригинала проще переносить.

### Авторы и лицензия
- **Оригинальный мод:** [Vampirism](https://github.com/TeamLapen/Vampirism) — maxanier, cheaterpaul и участники TeamLapen
- **Порт на Fabric:** ZombieOcupantDigital
- **Лицензия кода:** [LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0), как у оригинала. Исходный код форка публикуется вместе с релизами
- Текстуры и модели — от авторов Vampirism; их лицензия прямо разрешает использование в форках. Звуки распространяются по своим лицензиям (CC Attribution и др., см. оригинальный README)

Если вам нравится мод, поддержите оригинальных авторов: [vampirism.dev](https://vampirism.dev) · [Discord](https://discord.gg/wuamm4P)

---

## 🇬🇧 English

### What is this
**Vampirism Fabric** is a fork of Vampirism 1.10.17, ported from Forge to Fabric. All of the original content is kept: gameplay, balance, structures, mobs and mechanics behave the same as in the Forge version.

Vampires are fast, strong and bloodthirsty. They don't like the sun, but they don't fear the night, and the best part is that you can become one! Or grab a crossbow and some garlic and hunt them down instead.

### Features
- 🧛 **Two factions**: vampires and hunters, each with its own levels, skill trees and actions
- 🩸 **Blood instead of hunger**: feed on mobs and players, with a dedicated blood bar
- ☀️ **The sun is dangerous**: sunlight damage, with umbrellas, hoods and vampire clothing for protection
- 🌲 **Vampire Forest**: a new foggy biome with dark trees and unique flowers
- 🏰 **Structures**: baron castles, hunter camps and tents, faction totems in villages
- ⚔️ **Weapons and gear**: crossbows, hunter axes, vampire swords, armor, oils and potions
- 🧪 **Crafting**: alchemical cauldron, weapon table, altars, coffins, blood container and more
- 👥 **Minions, lords and tasks**: recruit helpers, complete tasks, rise in rank
- 🏘️ **Village capture**: bring villages over to your faction

### Requirements
| Dependency | Version |
|---|---|
| Minecraft | 1.20.1 |
| Fabric Loader | 0.16.14+ |
| [Fabric API](https://modrinth.com/mod/fabric-api) | 0.92.6+1.20.1 |
| Forge Config API Port | bundled, no separate install needed |

Required on both client and server.

### Differences from the original (known limitations)
- No **JEI**, **Guide-API** (guide book) or **TerraBlender** integration. The Vampire Forest is injected through Fabric API instead
- Vanilla **night vision** is not replaced with the vampire variant (visual only)
- The OBJ **bat cage** model is not rendered
- Key modifiers (Ctrl/Shift/Alt) for Vampirism hotkeys are not supported
- A few Forge-only cosmetic effects (running/landing particles, etc.) may differ
- Harmless `Unknown recipe category` warnings show up in the log

### How it works
The port bundles a compatibility layer that implements the parts of the Forge API Vampirism uses (events, registries, capabilities, networking, configs) on top of Fabric API and mixins. The original Vampirism code is left almost unchanged, which makes it easier to bring over upstream updates.

### Credits and license
- **Original mod:** [Vampirism](https://github.com/TeamLapen/Vampirism) by maxanier, cheaterpaul and the TeamLapen contributors
- **Fabric port:** ZombieOcupantDigital
- **Code license:** [LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0), same as the original. The fork's source code is published alongside every release
- Textures and models come from the Vampirism authors; their license explicitly allows use in forks. Sounds are under their own licenses (CC Attribution and others, see the original README)

If you enjoy the mod, please support the original authors: [vampirism.dev](https://vampirism.dev) · [Discord](https://discord.gg/wuamm4P)

# 📦 MidgardCore

**MidgardCore** är ett avancerat och optimerat kärnplugin utvecklat specifikt för Minecraft-servern **Midgard**. Pluginet samlar serverns mest centrala system i en enhetlig lösning – vilket eliminerar behovet av många separata plugins.

Med fokus på **prestanda, stabilitet och kontroll** innehåller MidgardCore funktioner som playtime-tracking, moderation, chatfilter, shop-system, inventory-hantering och full integration med PlaceholderAPI.

Genom att konsolidera funktionalitet i ett enda plugin får serverägare:

* ⚡ Bättre prestanda (mindre plugin-overhead)
* 🛠️ Enklare underhåll och felsökning
* 🔒 Centraliserad kontroll över alla system
* 🔗 Sömlös integration mellan funktioner

MidgardCore är byggt för att vara **skalbart, konfigurerbart och redo för större servrar**.

---

# 🎥 Video

[<img src="https://img.youtube.com/vi/KuJudqwtOqs/maxresdefault.jpg" alt="Se MidgardCore på YouTube" width="480">](https://www.youtube.com/watch?v=KuJudqwtOqs)

---

# 📚 Innehåll

* Kommandon
* Permissions
* Placeholders
* Systemöversikt

---

# 🧾 Kommandon

## 🎮 Spelarkommandon

| Kommando              | Beskrivning                    | Permission                        | Default |
| --------------------- | ------------------------------ | --------------------------------- | ------- |
| `/playtime`           | Visar spelarens totala speltid | `midgardcore.command.playtime`    | true    |
| `/playtimetop [sida]` | Visar topplista över playtime  | `midgardcore.command.playtimetop` | true    |

---

## 📢 Announcement

| Kommando               | Beskrivning                | Permission                         | Default |
| ---------------------- | -------------------------- | ---------------------------------- | ------- |
| `/announcement <text>` | Skickar globalt meddelande | `midgardcore.command.announcement` | op      |
| `/a <text>`            | Alias                      | samma                              | op      |

---

## 🎯 Gamemode

| Kommando             | Beskrivning            | Permission                     |
| -------------------- | ---------------------- | ------------------------------ |
| `/gm <0-3> [player]` | Sätter gamemode via ID | `midgardcore.command.gamemode` |
| `/gmc`               | Creative               | samma                          |
| `/gms`               | Survival               | samma                          |
| `/gmsp`              | Spectator              | samma                          |
| `/gma`               | Adventure              | samma                          |

---

## 🌤️ Tid & Väder

| Kommando | Beskrivning | Permission                    |
| -------- | ----------- | ----------------------------- |
| `/day`   | Sätter dag  | `midgardcore.command.time`    |
| `/night` | Sätter natt | `midgardcore.command.time`    |
| `/sun`   | Klart väder | `midgardcore.command.weather` |
| `/rain`  | Regn        | samma                         |

---

## 👻 Vanish

| Kommando           | Beskrivning       | Permission                   |
| ------------------ | ----------------- | ---------------------------- |
| `/vanish [player]` | Växlar osynlighet | `midgardcore.command.vanish` |
| `/v [player]`      | Alias             | samma                        |

---

## 🛒 Shop

| Kommando                               | Beskrivning         | Permission                 |
| -------------------------------------- | ------------------- | -------------------------- |
| `/shop create <name> <price> <amount>` | Skapar shop         | `midgardcore.command.shop` |
| `/shop edit <id> price <price>`        | Ändrar pris         | samma                      |
| `/shop edit <id> amount <amount>`      | Ändrar mängd        | samma                      |
| `/shop edit <id> toggle`               | Aktivera/inaktivera | samma                      |
| `/shop remove <id>`                    | Tar bort shop       | samma                      |
| `/shop info <player> [id]`             | Visar info          | samma                      |
| `/shop accept`                         | Accepterar köp      | samma                      |
| `/shop deny`                           | Nekar köp           | samma                      |

---

## 🎒 Inventory & Enderchest

| Kommando                    | Beskrivning      | Permission                               |
| --------------------------- | ---------------- | ---------------------------------------- |
| `/seeinventory <player>`    | Visa inventory   | `midgardcore.command.inventorysee.view`  |
| `/inventoryclear <player>`  | Rensa inventory  | `midgardcore.command.inventorysee.edit`  |
| `/seeenderchest <player>`   | Visa enderchest  | `midgardcore.command.enderchestsee.view` |
| `/enderchestclear <player>` | Rensa enderchest | `midgardcore.command.enderchestsee.edit` |

---

## 🔄 Reload

| Kommando              | Beskrivning      | Permission                   |
| --------------------- | ---------------- | ---------------------------- |
| `/midgardcore reload` | Laddar om plugin | `midgardcore.command.reload` |
| `/mc reload`          | Alias            | samma                        |

---

## 🛡️ Moderation

| Kommando                        | Beskrivning    | Permission                    |
| ------------------------------- | -------------- | ----------------------------- |
| `/ban <player> <reason> [time]` | Bannar spelare | `midgardcore.command.ban`     |
| `/kick <player> <reason>`       | Kickar         | `midgardcore.command.kick`    |
| `/warn <player> <reason>`       | Varnar         | `midgardcore.command.warn`    |
| `/mute <player>`                | Mutar          | `midgardcore.command.mute`    |
| `/unban <player>`               | Tar bort ban   | `midgardcore.command.unban`   |
| `/unmute <player>`              | Tar bort mute  | `midgardcore.command.unmute`  |
| `/history <type> <player>`      | Historik       | `midgardcore.command.history` |

---

## 💬 ChatFilter

| Kommando             | Beskrivning             | Permission                       |
| -------------------- | ----------------------- | -------------------------------- |
| `/chatfilter on`     | Aktiverar staff-visning | `midgardcore.command.chatfilter` |
| `/chatfilter off`    | Avaktiverar visning     | samma                            |
| `/chatfilter status` | Visar status            | samma                            |

---

# 🔐 Permissions

| Permission                               | Beskrivning                  |
| ---------------------------------------- | ---------------------------- |
| `midgardcore.command.*`                  | Alla kommandon               |
| `midgardcore.chatfilter.notify`          | Få notiser om filtrerade ord |
| `midgardcore.command.inventorysee.view`  | Visa inventory               |
| `midgardcore.command.inventorysee.edit`  | Redigera inventory           |
| `midgardcore.command.enderchestsee.view` | Visa enderchest              |
| `midgardcore.command.enderchestsee.edit` | Redigera enderchest          |

---

# 🧩 Placeholders

## ⏱️ Playtime

| Placeholder                     | Beskrivning |
| ------------------------------- | ----------- |
| `%midgardcore_playtime%`        | Total tid   |
| `%midgardcore_playtime_year%`   | År          |
| `%midgardcore_playtime_month%`  | Månader     |
| `%midgardcore_playtime_day%`    | Dagar       |
| `%midgardcore_playtime_hour%`   | Timmar      |
| `%midgardcore_playtime_minute%` | Minuter     |

---

## 📊 PlaytimeTop

| Placeholder     | Beskrivning        |
| --------------- | ------------------ |
| `%page%`        | Nuvarande sida     |
| `%total_pages%` | Totalt antal sidor |
| `%rank%`        | Ranking            |
| `%player%`      | Spelare            |
| `%playtime%`    | Speltid            |

---

## 📢 Announcement

| Placeholder | Beskrivning |
| ----------- | ----------- |
| `%message%` | Meddelande  |
| `%sender%`  | Avsändare   |

---

## 🛡️ Punishment System

| Placeholder    | Beskrivning |
| -------------- | ----------- |
| `%player%`     | Spelare     |
| `%target%`     | Mål         |
| `%staff%`      | Staff       |
| `%reason%`     | Anledning   |
| `%duration%`   | Tid         |
| `%time_left%`  | Tid kvar    |
| `%expires_at%` | Sluttid     |

---

# ⚙️ Systemöversikt

## 🛡️ Punishment System

* Fullt konfigurerbart system för moderation
* Stöd för: ban, mute, warn, kick
* Historik sparas per spelare

---

## 💬 ChatFilter

* Blockerar ord med valbara straff
* Stöd för leetspeak (t.ex. siffror istället för bokstäver)
* Fungerar i chat, privata meddelanden, skyltar, anvil och böcker
* Staff kan se filtrerade meddelanden i realtid
* Loggar sparas i fil eller MySQL

---

## 💥 Anti MobGriefing

* Creepers & ghasts förstör inte block
* Endermen kan inte flytta block
* Skyddar världen från grief

---

## 🎒 Inventory System

* Visa och redigera inventory (online/offline)
* Realtidssynk
* Stöd för YAML och MySQL

---

## 📦 Enderchest System

* Full kontroll över spelares enderchest
* Offline-stöd
* Realtidssynk

---

## 🛒 Shop System

* Exakt item-matchning (NBT)
* GUI-baserad handel
* Skydd mot exploits
* Automatisk cleanup

---

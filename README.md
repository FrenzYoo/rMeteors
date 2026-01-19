# rMeteors

rMeteors is an advanced, event-based Minecraft plugin that introduces scheduled meteor shower events with fully configurable mechanics, locations, rewards, and visuals. It is designed to feel vanilla-friendly while adding competitive and engaging gameplay to your server.

---

## ✨ Features

* ⏰ **Scheduled Events**
  Start events at specific times (e.g. 18:00, 20:00, 21:00) or disable scheduling entirely.

* 🛠️ **Editor-Based Locations**
  Admins define exact spawn locations using an editor command. All locations are saved to `data.yml` (world + coordinates).

* ☄️ **Simultaneous Meteor Spawns**
  When the event starts, meteors land at all defined locations at the same time.

* 🪨 **Layer Stone System**
  A Layer Stone spawns under each meteor block. Players cannot break Layer Stones, and they are removed automatically when the event ends or when the stone above is broken.

* 🧱 **Custom Core Stones**

  * Multiple block types supported
  * Each block has its own HP, rewards, and drop chances
  * Probability-based spawning (e.g. 40% / 60%)

* ⚒️ **Vanilla-Style Mining**

  * Stones spawn with full HP
  * Broken normally like Survival mode blocks
  * No creative-style instant breaking
  * Each successful block break removes exactly **1 HP**, regardless of tool

* 👑 **Ownership System**

  * First player to damage a stone becomes its owner
  * Ownership timer resets to 20 seconds on every hit
  * If the timer reaches 0, the stone has no owner

* 📊 **Hologram & Action Bar Support**

  * Displays stone name, remaining HP, and owner
  * Countdown updates every second
  * Fully configurable messages
  * Can be enabled or disabled via `config.yml`
  * Supports:

    * FancyHolograms
    * DecentHolograms
    * HolographicDisplays

* 💬 **Rich Chat Messages**

  * Event start & end messages
  * Countdown announcements before start
  * Player break messages (e.g. "Player X broke a stone, Y remaining")

* ⏳ **Event Duration**

  * Default: 5 minutes (configurable)
  * All stones are automatically removed when the event ends
  * `stop` command force-ends the event and removes all stones

---

## ⚙️ Commands

**Main command:** `/rmeteors`

| Subcommand  | Description                            |
| ----------- | -------------------------------------- |
| `start`     | Starts the meteor event                |
| `stop`      | Stops the event and removes all stones |
| `reload`    | Reloads config and data files          |
| `info`      | Shows plugin and event information     |
| `addloc`    | Adds a new meteor spawn location       |
| `removeloc` | Removes a specific spawn location      |
| `listlocs`  | Lists all saved spawn locations        |
| `clearlocs` | Removes all saved spawn locations      |

**Aliases:** `/rm`, `/meteor`
, `/meteor`

-------|-------------|
| `/rmeteors editor` | Enables editor mode to define spawn locations |
| `/rmeteors start` | Starts the meteor event |
| `/rmeteors stop` | Stops the event and removes all stones |
| `/rmeteors reload` | Reloads config and data files |

---

## 🔐 Permissions

* `rmeteors.admin` – Access to admin commands (start, stop, reload, location editor)
* `rmeteors.bypass` – Bypass ownership restrictions on stones

Default: **OP**

---

## 📁 Files

* `config.yml` – Main settings, blocks, rewards, messages, timings
* `data.yml` – Saved spawn locations

---

## 🔧 Requirements

* Spigot / Paper 1.16+
* Optional hologram plugin support (soft-depend):

  * FancyHolograms
  * DecentHolograms
  * HolographicDisplays

---

## 📌 Notes

* The old `base-damage` setting has been removed.
* Damage is strictly **1 HP per successful block break**.
* Events can only be restarted once all stones are removed.

---

## 🚀 Planned Additions

* BossBar support
* PlaceholderAPI support
* Per-world events
* Performance optimizations

---

## 🧑‍💻 Author

Developed for competitive and event-driven Minecraft servers.

Feel free to open issues or pull requests!

# rMeteors

---

---

## ✨ Features

* ⏰ **Scheduled Events**
  Start events at specific times (e.g. 18:00, 20:00, 21:00) or manually via command. Scheduled starts can be enabled or disabled from `config.yml`.

* ⏳ **Countdown System**
  A configurable countdown runs before the event starts. Messages and timings (e.g. 10m, 5m, 1m, 30s, 10s, 5s, 3s, 2s, 1s) are fully customizable.

* 🧩 **Placeholder Support**
  Use the placeholder `%rmeteors_countdown%` to display the remaining countdown time in scoreboards, holograms, or other supported plugins.

* 🛠️ **Editor-Based Locations**
  Admins define exact spawn locations using editor commands. All locations are saved to `data.yml` (world + coordinates).

* ☄️ **Simultaneous Meteor Spawns**
  When the event starts, meteors land at all defined locations at the same time.

* 🪨 **Layer Stone System**
  A Layer Stone spawns under each meteor block. Players cannot break Layer Stones, and they are removed automatically when the event ends or when the stone above is broken.

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

| Command | Description |
|-------|-------------|
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

<h1><img src="https://www.spigotmc.org/data/resource_icons/102/102275.jpg?1653755169" style="width: 20px; height:20px" /> Custom Enchantments 3 | Settings</h1>

This repository contains the plugin's default and custom configuration. You can also contribute by sharing your own plugin configuration for others to use.

### Server compatibility

CE3 runs on Spigot and Paper from 1.16.5 to 26.3, and on Folia from 1.19.4 to 26.3 (CE3 1.11.0 and newer). Java 16 or newer. A few parts need a newer Minecraft than 1.16.5, and on an older server they are switched off with a note to admins on join and to players who reach for them:

| Feature | Needs |
| --- | --- |
| Freeze effects on Freeze, Frost Arrow, Storm and Hail Storm | 1.17 |
| Companion Healing, Companion Thorns and the animal armor shop | 1.20.5 |
| Mace enchantments and the mace shop | 1.21 |
| Spear enchantments and the spear shop | 1.21.11 |

Set `VersionNotice: false` in config.yml to stop the admin note.

### Bedrock players

Bedrock players who join through Geyser can use every part of CE3. On Premium 1.13.0 and newer, with [Floodgate](https://geysermc.org/download#floodgate) installed on the server, they also get touch menus for the book shops instead of the chest: a list of shops, a list of books with their prices, and one book with its full description and a Buy button. Geyser and Floodgate are both optional; without Floodgate everyone uses the chest shop. Set `BedrockForms: false` in config.yml, or switch it off in `/ce setup`, to give Bedrock players the chest shop anyway. Lite always uses the chest shop.

### Histoblock

On CE3 1.15.0 and newer, with [Histoblock](https://www.jhprojects.dev/histoblock) 0.7.0 or newer installed, CE3 reads its history for tracking. Mining quests only count blocks no player placed, even across restarts, and a kill Minecraft gives no one credit for (TNT a player lit, for example) counts for the player who caused it, in kill quests and mob EXP. From CE3 1.15.1 with Histoblock 1.1.0, that kill is paid the moment the mob dies, and place quests skip a block placed where you broke your own placed block in the last 10 minutes. CE3 keeps all of its own data either way. Set `HistoblockSupport: false` in config.yml to leave it off.

### Quick start

Install the jar, start the server, join as an op and type `/ce setup`. The menu picks a play style, switches features on or off, places shops with one click and changes the common settings, all written into `config.yml` for you. The full guide is on the [plugin page](https://www.jhprojects.dev/customenchantments3).

### Configuration

- [config.yml](/config/default/config.yml) - `default` | v1.15.1

### Language

- [English](/languages/english/lang.yml) - English `default` | v1.13.0

Language packs, one per language, that each player can pick for themselves in `/ce settings` (CE3 1.10.0 and newer). See [languages/README.md](/languages/README.md) for how to install them.

| Code | Language | |
| --- | --- | --- |
| `de_de` | Deutsch (German) | [de_de.yml](/languages/packs/de_de.yml) |
| `es_es` | Español (Spanish) | [es_es.yml](/languages/packs/es_es.yml) |
| `fr_fr` | Français (French) | [fr_fr.yml](/languages/packs/fr_fr.yml) |
| `id_id` | Bahasa Indonesia (Indonesian) | [id_id.yml](/languages/packs/id_id.yml) |
| `ja_jp` | 日本語 (Japanese) | [ja_jp.yml](/languages/packs/ja_jp.yml) |
| `ko_kr` | 한국어 (Korean) | [ko_kr.yml](/languages/packs/ko_kr.yml) |
| `nl_nl` | Nederlands (Dutch), by Crumbless | [nl_nl.yml](/languages/packs/nl_nl.yml) |
| `pt_br` | Português (Brazilian Portuguese) | [pt_br.yml](/languages/packs/pt_br.yml) |
| `ru_ru` | Русский (Russian) | [ru_ru.yml](/languages/packs/ru_ru.yml) |
| `vi_vn` | Tiếng Việt (Vietnamese) | [vi_vn.yml](/languages/packs/vi_vn.yml) |
| `zh_cn` | 简体中文 (Simplified Chinese) | [zh_cn.yml](/languages/packs/zh_cn.yml) |

### Bandits

- [Bandits.yml](/bandits/default/bandits.yml) - `default` | v1.5.0

### Exp Config

- [ExpConfig.yml](/exp_config/default/ExpConfig.yml) - `default` | v1.0.0

### Loot Items

- [LootItems.yml](/loot_items/default/LootItems.yml) - `default` | v1.0.5

### Looting Plots

- [LootPlots.yml](/looting_plots/default/LootPlots.yml) - `default` | v1.0.7

### Resource Pack

- [CustomEnchantments 3 [1.16].zip](/resource_packs/§dCustomEnchantments%203%20[1.16].zip)
- [CustomEnchantments 3 [1.17].zip](/resource_packs/§dCustomEnchantments%203%20[1.17].zip)
- [CustomEnchantments 3 [1.18].zip](/resource_packs/§dCustomEnchantments%203%20[1.18].zip)
- [CustomEnchantments 3 [1.19].zip](/resource_packs/§dCustomEnchantments%203%20[1.19].zip)
- [CustomEnchantments 3 [1.21].zip](/resource_packs/§dCustomEnchantments%203%20[1.21].zip) [CE3 v1.3.0+]
- [CustomEnchantments 3 [26].zip](/resource_packs/§dCustomEnchantments%203%20[26].zip)

### Website

- [Custom Enchantments 3](https://www.jhprojects.dev/customenchantments3)

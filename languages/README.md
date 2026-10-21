# Custom Enchantments 3 languages

Since 1.10.0 a server can have more than one language. `lang.yml` is the built in one (English out of the box). Every pack in `plugins/CustomEnchantments3/languages/` is another, and each player picks their own in `/ce settings`. Nobody else's text changes when they do.

## Installing a pack

In game, as an op or with `customenchants.admin`:

```
/ce language install de_de
```

That downloads `languages/packs/de_de.yml` from this repository into the server's `languages` folder and loads it. Players can pick it straight away.

By hand, on a server that cannot reach GitHub:

1. Download the pack from [packs/](/languages/packs).
2. Put it in `plugins/CustomEnchantments3/languages/`, keeping its name (`de_de.yml`).
3. Run `/ce language reload`, or restart.

`/ce language` shows admins the same steps in game, along with what is installed, what is ready to install, and any file that failed to load and why.

## Ready made packs

| Code | Language |
| --- | --- |
| `de_de` | Deutsch (German) |
| `es_es` | Español (Spanish) |
| `fr_fr` | Français (French) |
| `id_id` | Bahasa Indonesia (Indonesian) |
| `ja_jp` | 日本語 (Japanese) |
| `ko_kr` | 한국어 (Korean) |
| `pt_br` | Português (Brazilian Portuguese) |
| `ru_ru` | Русский (Russian) |
| `vi_vn` | Tiếng Việt (Vietnamese) |
| `zh_cn` | 简体中文 (Simplified Chinese) |

`packs/index.yml` lists the same, and is what `/ce language` reads.

## What a player's language covers

Chat lines, titles, the action bar and every menu: shops, the skill tree, settings, the help pages, the treasure codex.

Text written onto an item stays in the server default, `DefaultLanguage` in `config.yml`. That covers enchantment names and levels in lore, treasure stats, potion and wand names, and book lore. Items change hands, and CE3 reads some of those lines back, so they are written in one language. Set `DefaultLanguage` to a pack's code to make that pack the language of the whole server, items included. On a server that already has enchanted items, the lore on those items stays in the old language.

## Resetting the built in language

[english/lang.yml](/languages/english/lang.yml) is `lang.yml` as CE3 1.10.0 writes it. Copy it over `plugins/CustomEnchantments3/lang.yml` to undo edits.

## Writing or fixing a pack

Copy any pack and change the `Language` block at the top. Name the file after a [Minecraft locale code](https://minecraft.wiki/w/Language), lower case, which is how the join notice matches a player's game language to a pack.

- Keep `_a`, `_b` and `_c` where they are. CE3 puts names and numbers there.
- Keep anything a player types exactly as it is: commands (`/ce settings`, `'/ce quest add'`) and the chat words `save`, `cancel`, `accept`, `deny`.
- A line you leave out is shown in the server default, so a partial pack works.

The plugin repository has `tools/language-packs.mjs`, which checks a pack against the English lines of the version you are on:

```
node tools/language-packs.mjs check <folder with the packs>
```

### Contributing

- Fork this repository.
- Add or fix a file in `languages/packs/`.
- Open a pull request and add [JayMar921](https://github.com/jaymar921) as a reviewer so it gets seen.

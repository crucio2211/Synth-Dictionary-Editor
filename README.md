# Synth Dictionary Editor

An NVDA add-on that lets you view and edit the pronunciation dictionary files (`.dic`) used by the **IBMTTS** and **Eloquence** synthesizers directly from within NVDA — no need to open a separate text editor or restart NVDA manually.

> **Note:** This is separate from NVDA's built-in Speech Dictionary (Preferences → Speech Dictionaries). This add-on edits the low-level `.dic` files read directly by the synthesizer engine itself.

---

## Compatibility

| Synthesizer | Notes |
|---|---|
| IBMTTS | Must be installed as an NVDA add-on. All versions supported. |
| Eloquence | Must be installed as an NVDA add-on. All versions supported. |

Requires **NVDA 2019.3 or later**.

---

## Features

- **Dictionary editor** — View, search, add, edit, and remove entries in any `.dic` file
- **Virtual list** — Fast rendering even with 65,000+ entries; no UI lag
- **Word variation generator** — Automatically generate morphological variations from a root word based on common affixes (prefixes, suffixes, infixes)
- **Single import** — Import entries from any `.dic` or `.txt` file into an existing or new dictionary
- **Batch import** — Import multiple files at once; files following the standard naming convention are matched automatically, others prompt for language and type assignment
- **Export** — Save any dictionary's entries to a file
- **Online dictionary update** — Download and merge entries from community-maintained GitHub repositories (Alternative IBM TTS Dictionaries or IBM TTS Dictionaries)
- **Auto-reload** — Synthesizer reloads automatically after saving, no NVDA restart needed
- **Multi-synth support** — If both IBMTTS and Eloquence are installed, you will be asked which one to edit on launch

---

## How to Open

**NVDA menu → Tools → Synth Dictionary Editor...**

---

## Dictionary File Naming Convention

Dictionary files follow the pattern: **`<langcode><type>.dic`**

### Language Codes

| Code | Language |
|---|---|
| `enu` | English (US) |
| `eng` | English (UK) |
| `esp` | Spanish (Spain) |
| `esm` | Spanish (Latin America) |
| `ptb` | Portuguese (Brazil) |
| `fra` | French (France) |
| `frc` | French (Canada) |
| `deu` | German |
| `ita` | Italian |
| `fin` | Finnish |
| `chs` | Chinese (Simplified) |
| `jpn` | Japanese |
| `kor` | Korean |

### Dictionary Types

| Suffix | Purpose |
|---|---|
| `main` | Main word pronunciation dictionary |
| `root` | Root word forms |
| `abbr` | Abbreviations and acronyms |

**Examples:** `enumain.dic`, `enuroot.dic`, `enuabbr.dic`, `ptbmain.dic`, `deuroot.dic`

---

## Phoneme Quick Reference

Entries can use two pronunciation formats:

### Spelled-Out
Write how the word sounds using words the synth already reads naturally. Best for acronyms.

```
OMG    oh em jee
NVDA   en vee dee ay
```

### Phoneme String
Wrap phoneme symbols in `` `[...] `` for precise phonetic control.

```
hello    `[.1hE.0lo]
computer `[k@m.1pyu.0ter]
```

**Stress markers:** `.1` = primary, `.2` = secondary, `.0` = unstressed

**Key vowels:** `A` (father), `a` (cat), `E` (bed), `I` (bit), `i` (beat), `O` (bought), `U` (book), `u` (boot), `@` (schwa)

**Key consonants:** `C` (ch), `D` (voiced th), `G` (ng), `J` (j/dge), `S` (sh), `T` (voiceless th), `Z` (zh/measure), `x` (loch)

See the full phoneme reference in the add-on's help file (NVDA Add-on Manager → Help).

---

## Online Dictionary Sources

The built-in update feature pulls from:

- [Alternative IBM TTS Dictionaries](https://github.com/mohamed00/AltIBMTTSDictionaries) by mohamed00
- [IBM TTS Dictionaries](https://github.com/eigencrow/IBMTTSDictionaries) by eigencrow

---

## Changelog

### v1.0
- Initial release
- Support for IBMTTS and Eloquence synthesizers
- Virtual list for fast loading of large dictionary files
- Search, add, edit, remove, import, batch import, export, and remove dictionary file features
- Word variation generator for morphological affixes
- Online dictionary update from community GitHub repositories
- Auto-reload synthesizer after saving

---

## License

GNU General Public License v2.0 — see [LICENSE](LICENSE) for details.

---

## Author

crucio2211

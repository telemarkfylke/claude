# TFK Claude-konfigurasjonsbibliotek

Delt Claude Code-konfigurasjon og ferdigheter for Telemark Fylke.

## Hva er i dette repoet

| Sti | Formål |
|-----|--------|
| `CLAUDE.md` | Delte teaminstruksjoner som lastes av Claude Code i hver sesjon |
| `skills/` | Teamspesifikke Claude-ferdigheter (slash-kommandoer) |
| `config/` | Eksempelkonfigurasjonsfiler for kopiering og tilpasning lokalt |

## Kom i gang

### 1. Kopier delt konfigurasjon

Kopier eksempelfilene til din lokale Claude-konfigurasjonsmappe og tilpass dem:

```bash
cp config/settings.example.json ~/.claude/settings.local.json
cp config/keybindings.example.json ~/.claude/keybindings.json
```

### 2. Installer ferdigheter

Kopier de ferdighetsfilene du ønsker til din lokale ferdighetsmappe:

```bash
cp skills/<ferdighetsnavn>.md ~/.claude/skills/
```

Eller symlenk hele mappen hvis du vil at endringer skal synkroniseres automatisk:

```bash
ln -s $(pwd)/skills ~/.claude/skills/tfk
```

### 3. Bruk CLAUDE.md

For prosjektrepoer, kopier eller symlenk `CLAUDE.md` til rotmappen i repoet slik at Claude automatisk henter teamkonvensjonene:

```bash
cp CLAUDE.md /path/to/your/project/CLAUDE.md
```

## Bidra

- Legg til nye ferdigheter i `skills/` med et beskrivende navn og tydelig frontmatter
- Hold `config/`-filer som eksempler — aldri commit ekte API-nøkler eller personlige stier
- Oppdater denne README-en når du legger til nytt innhold

# TFK Claude-konfigurasjonsbibliotek

Delt Claude Code-konfigurasjon og ferdigheter for Telemark Fylke.

## Innhold i dette repoet

| Sti | Formål |
|-----|--------|
| `CLAUDE.md` | Delte teaminstruksjoner som lastes av Claude Code i hver sesjon |
| `skills/` | Teamspesifikke Claude-ferdigheter (slash-kommandoer) |
| `config/` | Eksempelkonfigurasjonsfiler som kan kopieres og tilpasses lokalt |

## Kom i gang

### 1. Kopier delt konfigurasjon

Kopier eksempelfilene til din lokale Claude-konfigurasjonskatalog og tilpass dem:

```bash
cp config/settings.example.json ~/.claude/settings.local.json
cp config/keybindings.example.json ~/.claude/keybindings.json
```

### 2. Installer ferdigheter

Kopier ønskede ferdighetsfiler til din lokale ferdighetskatalog:

```bash
cp skills/<ferdighetsnavn>.md ~/.claude/skills/
```

Eller lag en symbollenke til hele mappen hvis du vil at endringer skal synkroniseres automatisk:

```bash
ln -s $(pwd)/skills ~/.claude/skills/tfk
```

### 3. Bruk CLAUDE.md

For prosjektrepoer, kopier eller lenk `CLAUDE.md` til roten av repoet slik at Claude automatisk plukker opp teamkonvensjoner:

```bash
cp CLAUDE.md /path/to/your/project/CLAUDE.md
```

## Bidra

- Legg til nye ferdigheter i `skills/` med et beskrivende navn og tydelig frontmatter
- Hold `config/`-filer som eksempler — commit aldri ekte API-nøkler eller personlige stier
- Oppdater denne README når du legger til nytt innhold

# 🤖 TFK Claude-konfigurasjonsbibliotek

Delt Claude Code-konfigurasjon og ferdigheter for Telemark Fylke.

## 📦 Hva er i dette repoet

| Sti | Formål |
|-----|--------|
| `CLAUDE.md` | Delte teaminstruksjoner lastet av Claude Code i hver sesjon |
| `skills/` | Teamspesifikke Claude-ferdigheter (slash-kommandoer) |
| `config/` | Eksempelkonfigurasjonsfiler for lokal kopiering og tilpasning |

## 🚀 Kom i gang

### 1. 📋 Kopier delt konfigurasjon

Kopier eksempelfilene til din lokale Claude-konfigurasjonskatalog og tilpass dem:

```bash
cp config/settings.example.json ~/.claude/settings.local.json
cp config/keybindings.example.json ~/.claude/keybindings.json
```

### 2. 🛠️ Installer ferdigheter

Kopier ferdighetsfiler du ønsker til din lokale ferdighetsmappe:

```bash
cp skills/<skill-name>.md ~/.claude/skills/
```

Eller lag en symbolkobling til hele mappen hvis du vil at endringer skal synkroniseres automatisk:

```bash
ln -s $(pwd)/skills ~/.claude/skills/tfk
```

### 3. 📄 Bruk CLAUDE.md

For prosjektrepoer, kopier eller lag en symbolkobling til `CLAUDE.md` i rotmappen slik at Claude automatisk plukker opp teamkonvensjonene:

```bash
cp CLAUDE.md /path/to/your/project/CLAUDE.md
```

## 🤝 Bidrag

- Legg til nye ferdigheter i `skills/` med et beskrivende navn og tydelig frontmatter
- Hold `config/`-filene som eksempler — commit aldri ekte API-nøkler eller personlige stier
- Oppdater denne README når du legger til nytt innhold

---

> 💡 **Dagens vits:** Hva er den største løgnen i IT?
> *«Dokumentasjonen er oppdatert.»* 😄

---

Laget med ❤️ i TFK

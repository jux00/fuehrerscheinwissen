# Obsidian Markdown Referenz

Kompakte Referenz für Agents zur Erstellung von Obsidian-kompatiblen Notizen.

---

## Links

```markdown
[[Dateiname]]                    # Link zu anderer Notiz
[[Dateiname|Anzeigetext]]        # Link mit custom Text
[[Dateiname#Überschrift]]        # Link zu Abschnitt
[[Dateiname#^block-id]]          # Link zu Block
![[Dateiname]]                   # Embed (einbetten)
![[Bild.png]]                    # Bild einbetten
![[Bild.png|300]]                # Bild mit Breite
[Externer Link](https://...)     # Externer Link
```

---

## Tags

```markdown
#tag                             # Einfacher Tag
#kategorie/unterkategorie        # Nested Tag
```

Konvention für Führerschein-Projekt:
- `#prüfung` - Prüfungsrelevant
- `#zahlen` - Enthält wichtige Zahlen
- `#formel` - Enthält Formeln
- `#merksatz` - Eselsbrücken

---

## Formatierung

```markdown
**fett**
*kursiv*
~~durchgestrichen~~
==markiert/highlighted==
`code inline`
> Zitat/Blockquote
---                              # Horizontale Linie
```

---

## Überschriften

```markdown
# H1
## H2
### H3
#### H4
```

---

## Listen

```markdown
- Punkt 1
- Punkt 2
  - Unterpunkt

1. Nummeriert
2. Zweiter Punkt

- [ ] Checkbox leer
- [x] Checkbox erledigt
```

---

## Tabellen

```markdown
| Spalte 1 | Spalte 2 | Spalte 3 |
|----------|:--------:|---------:|
| Links    | Zentriert| Rechts   |
| Daten    | Daten    | Daten    |
```

Ausgabe:
| Spalte 1 | Spalte 2 | Spalte 3 |
|----------|:--------:|---------:|
| Links    | Zentriert| Rechts   |

---

## Callouts

### Syntax

```markdown
> [!TYPE] Optionaler Titel
> Inhalt des Callouts
> Kann mehrere Zeilen haben
```

### Faltbar (Collapsible)

```markdown
> [!TYPE]+ Standardmäßig offen
> Inhalt

> [!TYPE]- Standardmäßig geschlossen
> Inhalt
```

### Alle Callout-Typen

| Typ | Aliase | Farbe | Verwendung |
|-----|--------|-------|------------|
| `note` | - | Grau | Allgemeine Notizen |
| `abstract` | `summary`, `tldr` | Türkis | Zusammenfassungen |
| `info` | `todo` | Blau | Informationen |
| `tip` | `hint`, `important` | Türkis | Tipps, Hinweise |
| `success` | `check`, `done` | Grün | Erfolg, erledigt |
| `question` | `help`, `faq` | Gelb | Fragen |
| `warning` | `caution`, `attention` | Orange | Warnungen |
| `failure` | `fail`, `missing` | Rot | Fehler |
| `danger` | `error` | Rot | Gefahr |
| `bug` | - | Rot | Bugs |
| `example` | - | Lila | Beispiele |
| `quote` | `cite` | Grau | Zitate |

### Beispiele für Führerschein-Notizen

```markdown
> [!tip] Merksatz
> Rechts vor links gilt NICHT auf Vorfahrtsstraßen!

> [!warning] Achtung
> Bei Nebel: Sichtweite = maximale Geschwindigkeit

> [!info] Zahlen
> Innerorts: 50 km/h | Außerorts: 100 km/h | Autobahn: Richtgeschwindigkeit 130

> [!example] Beispielrechnung
> Anhalteweg bei 50 km/h:
> - Reaktionsweg: (50÷10) × 3 = 15m
> - Bremsweg: (50÷10)² = 25m
> - **Anhalteweg: 40m**

> [!danger] Prüfungsfalle
> Andreaskreuz = Vorfahrt für Schienenfahrzeuge!

> [!abstract] Zusammenfassung
> Die 3 wichtigsten Promillegrenzen: 0,0 (Probezeit) | 0,5 (normal) | 1,1 (absolut fahruntüchtig)
```

---

## Code-Blöcke

````markdown
```sprache
Code hier
```
````

---

## Mathematik (LaTeX)

```markdown
$E = mc^2$                       # Inline
$$
\frac{v}{10} \times 3 = Reaktionsweg
$$                               # Block
```

---

## Frontmatter (YAML)

```markdown
---
tags:
  - prüfung
  - geschwindigkeit
aliases:
  - Tempo
  - Speed
---
```

---

## Best Practices für Führerschein-Vault

1. **Dateinamen**: `XX - Thema.md` (nummeriert für Sortierung)
2. **Tags konsistent**: Immer gleiche Tags verwenden
3. **Callouts für**:
   - `[!tip]` → Merksätze, Eselsbrücken
   - `[!warning]` → Häufige Fehler
   - `[!info]` → Wichtige Zahlen
   - `[!example]` → Beispielrechnungen
   - `[!danger]` → Prüfungsfallen
   - `[!abstract]` → Zusammenfassungen
4. **Tabellen** für Zahlenübersichten
5. **Verlinkungen** zwischen verwandten Themen

---

## Quellen

- [Obsidian Help - Basic Formatting](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax)
- [Obsidian Help - Advanced Formatting](https://help.obsidian.md/Editing+and+formatting/Advanced+formatting+syntax)
- [Face Dragons - Obsidian Markdown Cheatsheet](https://facedragons.com/personal-development/obsidian-markdown-cheatsheet/)

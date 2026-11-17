# Prozess-Skill

Ein Skill für Claude. Der Prozess-Skill findet die Zeitfresser in deiner Woche und schlägt passende Automatisierungen vor, schreibt Stellenanzeige, Interviewfragen und Probeaufgabe für deine erste Aushilfe und baut Briefings, mit denen Designer und Texter beim ersten Mal liefern. Du erklärst einen Ablauf einmal laut, und Claude macht daraus eine Anleitung, mit der es jede Aushilfe ab morgen allein kann. Kostenlos, MIT-Lizenz.

| Modul | Was es macht |
| --- | --- |
| **Zeitfresser-Analyse** | Deine Woche als Tabelle mit Stunden pro Monat, jede Aufgabe eingeordnet: weglassen, automatisieren, delegieren, vereinfachen oder behalten. |
| **Recruiting-Kit** | Stellenanzeige nach AGG, Interviewleitfaden mit Bewertungsbogen, Probeaufgabe und Einarbeitungsplan für die erste Woche. |
| **Briefings** | Ein- bis zweiseitiges Briefing mit Ziel, Lieferumfang, Stil, Rahmen und Nutzungsrechten, plus Begleitmail. |
| **Anleitungen** | Aus Sprachmemo oder Bildschirmaufnahme wird eine nummerierte Anleitung mit Entscheidungen, Prüfpunkten und typischen Fehlern, plus Checkliste. |

## Installation

### Claude-App (Web, Desktop)

Am schnellsten: den Link in einen neuen Chat einfügen und Claude bitten, den Skill zu installieren:

```
https://github.com/Ultra-Smashed/prozess-skill

Installier diesen Skill für mich.
```

Oder von Hand:

1. [`prozess.zip`](https://github.com/Ultra-Smashed/prozess-skill/raw/main/prozess.zip) herunterladen (nicht entpacken).
2. In Claude unter **Settings → Capabilities** den Schalter **Code execution and file creation** einschalten. In der neueren Ansicht heißt er **Create and edit files**.
3. **Customize → Skills** öffnen, auf **+** klicken, dann **Create skill → Upload a skill** und die ZIP-Datei wählen.

Als Plugin: **Customize → Plugins**, bei den persönlichen Plugins auf **+**, dann **Add from a repository** und `Ultra-Smashed/prozess-skill` eintragen.

Die Menünamen stehen hier so, wie Anthropic sie in der Hilfe nennt. In der deutschen Oberfläche können sie übersetzt sein.

### Claude Code

Als Plugin:

```
/plugin marketplace add Ultra-Smashed/prozess-skill
/plugin install prozess@prozess
```

Oder den Ordner kopieren:

```bash
git clone https://github.com/Ultra-Smashed/prozess-skill.git
cp -r prozess-skill/skills/prozess ~/.claude/skills/
```

## Benutzen

Einfach schreiben, was du brauchst, zum Beispiel:

> Ich erkläre dir jetzt, wie ich ein Angebot rausschicke. Mach daraus eine Anleitung für meine Aushilfe.

> Hier ist meine typische Woche. Wo verliere ich die meiste Zeit, und was kann ich automatisieren?

> Ich suche eine Assistenz für 10 Stunden die Woche, remote. Mach mir das Recruiting-Kit.

Der Test für jede Anleitung: Lass sie einmal von jemand anderem ausführen und schreib jede Rückfrage auf. Jede Rückfrage ist eine Lücke, die Claude dann schließt.

## Dateien

```
skills/prozess/SKILL.md            Ablauf, Module, Regeln
skills/prozess/modes/               eine Anleitung pro Modul
prozess.zip                       derselbe Skill-Ordner als ZIP für die Claude-App
.claude-plugin/                     plugin.json, marketplace.json
```

Nach einer Änderung im Skill-Ordner die ZIP neu bauen: `cd skills && zip -r ../prozess.zip prozess`.

Anleitung: [thanisch.co/wissen/guides/prozess-skill-claude](https://thanisch.co/wissen/guides/prozess-skill-claude)

MIT-Lizenz, siehe [LICENSE](LICENSE). Von [Christopher Thanisch](https://thanisch.co).

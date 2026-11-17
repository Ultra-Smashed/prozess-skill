# Modul Zeitfresser-Analyse

Ziel: Der Mensch sieht, wo in seiner Woche die meiste Zeit verloren geht, und bekommt passende Automatisierungen vorgeschlagen.

## Eingabe (eine der folgenden)

- Eine typische Woche beschreiben lassen (Tag für Tag, grob)
- Kalender-Export oder verbundenes Kalender-Werkzeug (nur lesen)
- Zeiterfassung (CSV)
- Liste wiederkehrender Aufgaben mit geschätzter Dauer

Dazu fragen: Welche Werkzeuge nutzt du (Mail, Kalender, Buchhaltung, CRM, Shop, Social)? Was nervt dich am meisten?

## Ablauf

1. **Aufgaben-Inventar** als Tabelle: Aufgabe · wie oft · Dauer · Stunden pro Monat (mit Code) · Kategorie (Kundenarbeit, Akquise, Verwaltung, Kommunikation, Sonstiges).
2. **Bewerten** je Aufgabe:
   - **Weglassen?** (bringt nichts)
   - **Automatisieren?** (regelbasiert, wiederholt, digital)
   - **Delegieren?** (braucht Menschen, aber nicht den Menschen selbst)
   - **Vereinfachen?** (Vorlage, Bündeln, feste Zeiten)
   - **Behalten** (Kern, macht Spaß, bringt Geld)
3. **Automatisierungen vorschlagen**, nur mit Werkzeugen, die es gibt und die zum Menschen passen. Je Vorschlag: was genau passiert, womit (z. B. Buchhaltungsprogramm-Funktion, Zapier/Make/n8n, Kalender-Buchungslink, E-Mail-Vorlagen, Claude-Skill), Aufwand zum Einrichten, gesparte Stunden pro Monat (Schätzung, gekennzeichnet).
   Typische Treffer: Terminbuchung statt Mail-Pingpong, wiederkehrende Rechnungen, Belege per Mail an die Buchhaltung, Formular statt Rückfragen, Vorlagen für Standardantworten, Social-Planung im Voraus.
4. **Ergebnis:**
   - Top 5 nach gesparter Zeit pro Monat im Verhältnis zum Aufwand
   - Summe gesparter Stunden (mit Code)
   - Für den ersten Vorschlag: konkrete Einrichtungs-Schritte
   - Was delegiert werden kann → Modul Anleitungen und Recruiting

Ehrlich: Schätzungen als Schätzungen. Keine Werkzeuge empfehlen, die man nicht kennt.

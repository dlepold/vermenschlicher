# AGENTS.md — Vermenschlicher

Dieses Repository enthält ein Skill für KI-Coding-Agenten (Claude Code, OpenCode).

## Was es ist

Ein Lektor-Skill, das Anzeichen für KI-generierten **deutschen** Text erkennt und entfernt.
Die gesamte Logik steht in [`SKILL.md`](SKILL.md).

## Aufruf

- Slash-Befehl: `/vermenschlicher` gefolgt vom Text.
- Oder per Bitte: „Vermenschliche diesen Text: …".
- Optionale Stimmen-Kalibrierung: eine eigene Schreibprobe mitgeben (siehe `SKILL.md`).

## Kernregel für Agenten

Anders als englische Humanizer wird der **Gedankenstrich im Deutschen NICHT pauschal
entfernt** — er ist legitimes Stilmittel. Verdächtig ist nur der Geviertstrich „—" (statt
„– " mit Leerzeichen) und gehäufter Einsatz. Siehe Muster #14 in `SKILL.md`.

## Vorgehen

Entwurf → Audit („Was macht das noch KI-haft?") → Endfassung. Bedeutung und Umfang bewahren,
nichts ersatzlos streichen.

## Quellen

Gegründet auf *Wikipedia:Anzeichen für KI-generierte Inhalte* (de.WP) und auf der Struktur
von [blader/humanizer](https://github.com/blader/humanizer). Details in `README.md`.

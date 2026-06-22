# Vermenschlicher

Ein Skill für **Claude Code** und **OpenCode**, der Anzeichen für KI-generierten
**deutschen** Text entfernt und ihn natürlicher und menschlicher klingen lässt.

Die deutsche Schwesterversion von [blader/humanizer](https://github.com/blader/humanizer) —
keine Übersetzung, sondern eigenständig gegründet auf die Seite
[*Wikipedia:Anzeichen für KI-generierte Inhalte*](https://de.wikipedia.org/wiki/Wikipedia:Anzeichen_f%C3%BCr_KI-generierte_Inhalte)
der deutschsprachigen Wikipedia.

> **Warum keine reine Übersetzung?** Deutsche KI-Tells unterscheiden sich von englischen.
> Das wichtigste Beispiel: Der **Gedankenstrich ist im Deutschen ein legitimes Stilmittel**
> und wird hier *nicht* pauschal gestrichen (anders als in englischen Humanizern) — verdächtig
> ist nur der falsch gesetzte Geviertstrich „—" und gehäufter Einsatz. Wer englische Regeln
> blind überträgt, macht den Text falscher, nicht besser.

## Installation

### Claude Code

Direkt ins Skills-Verzeichnis von Claude Code klonen:

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/dlepold/vermenschlicher.git ~/.claude/skills/vermenschlicher
```

Oder die Skill-Datei manuell kopieren, wenn das Repo schon geklont ist:

```bash
mkdir -p ~/.claude/skills/vermenschlicher
cp SKILL.md ~/.claude/skills/vermenschlicher/
```

### OpenCode

```bash
mkdir -p ~/.config/opencode/skills
git clone https://github.com/dlepold/vermenschlicher.git ~/.config/opencode/skills/vermenschlicher
```

> **Hinweis:** OpenCode durchsucht auch `~/.claude/skills/`. Wer beide Tools nutzt, kommt mit
> einem einzigen Klon nach `~/.claude/skills/vermenschlicher/` aus.

## Verwendung

```
/vermenschlicher

[Text hier einfügen]
```

Oder das Modell direkt bitten:

```
Vermenschliche diesen Text: [dein Text]
```

### Stimmen-Kalibrierung

Um den eigenen Schreibstil zu treffen, eine Probe mitgeben:

```
/vermenschlicher

Hier eine Schreibprobe zur Stil-Kalibrierung:
[2–3 Absätze deines eigenen Textes]

Jetzt vermenschliche diesen Text:
[KI-Text zum Vermenschlichen]
```

Das Skill analysiert Satzrhythmus, Wortwahl und Eigenheiten und überträgt sie auf die
Umschreibung, statt generisch „sauberen" Text zu produzieren.

## Was es erkennt

Rund 28 deutsche Muster mit Vorher/Nachher-Beispielen, u. a.:

| Bereich | Beispiele |
|---|---|
| **Lieblingswörter** | nahtlos, ganzheitlich, facettenreich, maßgeschneidert, **meistern**, bereichern, zukunftsweisend |
| **Floskeln** | „Tauchen wir ein", „In der heutigen schnelllebigen Welt", „Es ist wichtig zu beachten, dass", „Zusammenfassend lässt sich sagen", „Ob X oder Y – …" |
| **Struktur** | Trikolon, „nicht nur … sondern auch", Konjunktionen-Flut, Nominalstil/Behördendeutsch, Rhythmus-Monotonie |
| **Stil** | Geviertstrich-Spam (DE-Sonderregel!), übermäßige Fettschrift, Emojis, falsche Anführungszeichen |
| **Chatbot-Reste** | „Gerne!", „Ich hoffe, das hilft!", Wissensstands-Disclaimer, servil-höflicher Ton |
| **Werbesprache** | reiches kulturelles Erbe, atemberaubend, eingebettet, im Herzen von |

Die volle Liste mit Beispielen steht in [`SKILL.md`](SKILL.md).

## Quellen

- [Wikipedia:Anzeichen für KI-generierte Inhalte](https://de.wikipedia.org/wiki/Wikipedia:Anzeichen_f%C3%BCr_KI-generierte_Inhalte) — Primärquelle (de.WP)
- [blader/humanizer](https://github.com/blader/humanizer) — englisches Original, Struktur-Vorlage
- [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- Weber-Wulff et al. (2023), *Testing of detection tools for AI-generated text* — [arXiv:2306.15666](https://arxiv.org/abs/2306.15666)
- Fiedler et al. (2025), *ScienceDirect*; Doru et al. (2025), *JMIR Medical Education*

## Lizenz

MIT. Abgeleitet von [blader/humanizer](https://github.com/blader/humanizer) (ebenfalls MIT).
Siehe [LICENSE](LICENSE).

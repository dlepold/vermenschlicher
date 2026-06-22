---
name: vermenschlicher
version: 1.0.0
description: |
  Entfernt Anzeichen für KI-generierten deutschen Text und macht ihn natürlich
  und menschlich klingend. Einsetzen beim Bearbeiten oder Prüfen deutscher Texte.
  Gegründet auf "Wikipedia:Anzeichen für KI-generierte Inhalte" (de.wikipedia) und
  Studien zur KI-Texterkennung. Erkennt und behebt deutsche Muster: aufgeblähte
  Bedeutung, Werbesprache, KI-Lieblingswörter (nahtlos, ganzheitlich, facettenreich,
  meistern), Kopula-Vermeidung, Trikolon, "nicht nur ... sondern auch", Floskeln
  ("Tauchen wir ein", "In der heutigen schnelllebigen Welt", "Zusammenfassend ..."),
  Konjunktionen-Flut, Nominalstil/Behördendeutsch und Rhythmus-Monotonie. Anders als
  englische Humanizer: der Gedankenstrich wird NICHT pauschal gestrichen (im Deutschen
  legitim) — nur der falsch gesetzte Geviertstrich.
license: MIT
compatibility: claude-code opencode
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Vermenschlicher: KI-Schreibmuster aus deutschen Texten entfernen

Du bist ein Lektor, der Anzeichen für KI-generierten **deutschen** Text erkennt und
entfernt, damit das Geschriebene natürlich und von einem Menschen verfasst klingt.
Dieser Leitfaden fußt auf der Seite *„Wikipedia:Anzeichen für KI-generierte Inhalte"*
der deutschsprachigen Wikipedia (gepflegt im Rahmen der KI-Qualitätssicherung) sowie
auf linguistischer und journalistischer Forschung zur KI-Texterkennung im Deutschen.

> **Wichtig — keine Übersetzung eines englischen Skills.** Deutsche KI-Tells sind
> teils andere als englische. Insbesondere ist der **Gedankenstrich im Deutschen ein
> legitimes Stilmittel** und darf NICHT pauschal gestrichen werden (siehe Muster #14).
> Wer einfach englische Regeln überträgt, macht den Text *falscher*, nicht besser.

## Deine Aufgabe

Wenn dir ein Text zum Vermenschlichen gegeben wird:

1. **KI-Muster erkennen** — den Text gegen die unten gelisteten Muster scannen.
2. **Umschreiben, nicht löschen** — KI-Floskeln durch natürliche Formulierungen
   ersetzen und alles abdecken, was das Original abdeckt. Fünf Absätze bleiben fünf Absätze.
3. **Bedeutung bewahren** — die Kernaussage bleibt erhalten.
4. **Die Stimme treffen** — zum gewünschten Ton passen (förmlich, locker, technisch).
   Persönlichkeit nur dort hinzufügen, wo Inhalt und Autorenstimme es verlangen
   (siehe PERSÖNLICHKEIT UND SEELE).

Die Schleife Entwurf → Audit → Endfassung und das Ergebnis sind unter „Vorgehen und
Ausgabe" definiert.

## Stimmen-Kalibrierung (optional)

Wenn der Nutzer eine Schreibprobe (eigener früherer Text) mitgibt, analysiere sie zuerst:

1. **Probe zuerst lesen.** Achte auf:
   - Satzlängen-Muster (kurz und knackig? Lang und fließend? Gemischt?)
   - Wortwahl-Niveau (umgangssprachlich? akademisch? dazwischen?)
   - Absatzanfänge (direkt zur Sache? erst Kontext setzen?)
   - Zeichensetzungs-Gewohnheiten (viele Gedankenstriche? Klammer-Einschübe? Semikola?)
   - Wiederkehrende Wendungen oder Eigenheiten
   - Übergänge (explizite Konnektoren? oder einfach der nächste Punkt?)

2. **Diese Stimme in der Umschreibung treffen.** KI-Muster nicht nur entfernen, sondern
   durch Muster aus der Probe ersetzen. Schreibt der Autor kurze Sätze, mach keine langen.
   Benutzt er „Sachen" und „Dinge", werte nicht zu „Elemente" und „Komponenten" auf.

3. **Ohne Probe** greift das Standardverhalten (natürliche, abwechslungsreiche, meinungs-
   starke Stimme aus dem Abschnitt PERSÖNLICHKEIT UND SEELE).

### Probe übergeben
- Inline: „Vermenschliche diesen Text. Hier eine Schreibprobe zur Stil-Kalibrierung: [Probe]"
- Datei: „Vermenschliche diesen Text. Nutze meinen Schreibstil aus [Dateipfad] als Referenz."

## PERSÖNLICHKEIT UND SEELE

KI-Muster zu vermeiden ist nur die halbe Arbeit. Steriles, stimmloses Schreiben ist genauso
verräterisch wie Slop. Gutes Schreiben hat einen Menschen dahinter.

**Diesen Abschnitt nur anwenden, wenn Inhalt und Autorenstimme es verlangen** — Blogposts,
Essays, Meinung, persönliche Texte. Für enzyklopädische, technische, juristische oder
Referenztexte *ist* neutral und schlicht die richtige menschliche Stimme; dort keine
Meinungen oder Ich-Perspektive einstreuen.

### Anzeichen für seelenloses Schreiben (auch wenn technisch „sauber"):
- Jeder Satz hat dieselbe Länge und Struktur
- Keine Meinung, nur neutrales Referieren
- Kein Eingeständnis von Unsicherheit oder gemischten Gefühlen
- Keine Ich-Perspektive, wo sie passen würde
- Kein Humor, keine Kante, keine Persönlichkeit
- Liest sich wie ein Wikipedia-Artikel oder eine Pressemitteilung

### Wie man Stimme hinzufügt:

**Hab eine Meinung.** Fakten nicht nur referieren, sondern darauf reagieren. „Ich weiß
ehrlich nicht, was ich davon halten soll" ist menschlicher als das neutrale Auflisten von
Pro und Contra.

**Variiere den Rhythmus.** Kurze, knappe Sätze. Dann längere, die sich Zeit nehmen, bis sie
ankommen, wo sie hinwollen. Misch es.

**Lass etwas Unordnung zu.** Perfekte Struktur wirkt algorithmisch. Abschweifungen,
Einschübe und halbfertige Gedanken sind menschlich.

---

## INHALTLICHE MUSTER

### 1. Übertriebene Betonung von Bedeutung, Vermächtnis und großen Trends

**Wörter, auf die man achtet:** spielt eine entscheidende/zentrale/wichtige Rolle,
unterstreicht/hebt die Bedeutung hervor, ein Zeugnis für, markiert einen Wendepunkt,
bleibendes Vermächtnis, tief verwurzelt, im Wandel der Zeit, prägt die, ebnet den Weg für,
spiegelt einen größeren Trend wider

**Problem:** KI bläht Wichtigkeit auf, indem sie banale Aspekte zu Repräsentanten eines
großen Ganzen erklärt.

**Vorher:**
> Die Gründung des Vereins im Jahr 1989 markierte einen entscheidenden Wendepunkt in der
> Entwicklung des regionalen Vereinswesens und spiegelt einen größeren gesellschaftlichen
> Wandel hin zu bürgerschaftlichem Engagement wider.

**Nachher:**
> Der Verein wurde 1989 gegründet, um Sportangebote im Stadtteil zu organisieren.

### 2. Werbesprache und Hochglanz-Ton

**Wörter, auf die man achtet:** reiches kulturelles Erbe, reiche Geschichte, atemberaubend,
unbedingt besuchen/sehen, beeindruckende natürliche Schönheit, bleibendes Vermächtnis,
eingebettet, im Herzen von, malerisch, ein wahres Highlight, einzigartig
*(direkt aus der de.WP-Liste „Werbesprache")*

**Problem:** LLMs halten besonders bei „Kultur-" und Ortsthemen kaum einen neutralen Ton.

**Vorher:**
> Eingebettet im Herzen der atemberaubenden Eifel besticht das malerische Städtchen mit
> seinem reichen kulturellen Erbe und einer beeindruckenden natürlichen Schönheit.

**Nachher:**
> Die Stadt liegt in der Eifel und ist für ihren Wochenmarkt und die Kirche aus dem
> 18. Jahrhundert bekannt.

### 3. Oberflächliche Partizip-Analysen (-end/-ung)

**Wörter, auf die man achtet:** verdeutlichend, unterstreichend, betonend, widerspiegelnd,
sicherstellend, beitragend zu, fördernd, was zeigt/verdeutlicht, um zu gewährleisten

**Problem:** KI hängt Partizipial- und „um zu"-Konstruktionen an, um Tiefe vorzutäuschen.

**Vorher:**
> Die Farbgebung in Blau, Grün und Gold greift die Natur der Region auf und symbolisiert
> die Verbundenheit der Gemeinde mit dem Land, was ihre Identität widerspiegelt.

**Nachher:**
> Die Fassade ist blau, grün und gold. Der Architekt wählte diese Farben nach Vorbild der
> lokalen Landschaft.

### 4. Vage Autoritäten und Weasel-Wörter

**Wörter, auf die man achtet:** Experten sind sich einig, Beobachter weisen darauf hin,
Studien zeigen (ohne Quelle), viele Fachleute betonen, es wird angenommen, gilt als

**Problem:** KI schreibt Meinungen vagen Autoritäten zu, ohne konkrete Quelle.

**Vorher:**
> Experten sind sich einig, dass der Fluss eine entscheidende Rolle im regionalen Ökosystem
> spielt.

**Nachher:**
> Laut einer Erhebung der Universität Trier von 2019 leben im Fluss mehrere endemische
> Fischarten.

### 5. Formelhafte „Herausforderungen / Zukunftsaussichten"-Abschnitte

**Wörter, auf die man achtet:** Trotz seiner/dieser Erfolge … steht vor Herausforderungen,
Zukunftsaussichten, Herausforderungen und Chancen
*(de.WP: „Schlussfolgerungen")*

**Problem:** Viele KI-Texte hängen einen formelhaften „Herausforderungen"-Block an, der mit
einer vagen positiven Bewertung oder Spekulation endet.

**Vorher:**
> Trotz seiner wirtschaftlichen Erfolge steht der Ort vor Herausforderungen wie Verkehr und
> Wasserknappheit. Doch mit seiner strategischen Lage blickt er in eine vielversprechende
> Zukunft.

**Nachher:**
> Seit 2015 nahm der Verkehr zu, nachdem drei Gewerbegebiete erschlossen wurden. 2022 begann
> die Gemeinde ein Kanalprojekt gegen wiederkehrende Überschwemmungen.

---

## SPRACH- UND GRAMMATIKMUSTER

### 6. Überstrapaziertes „KI-Vokabular"

**Hochfrequente KI-Wörter (oft aus dem Englischen kalkiert):** nahtlos *(seamless)*,
ganzheitlich *(holistic)*, facettenreich/vielschichtig, maßgeschneidert *(tailored)*,
zukunftsweisend, entscheidend/essenziell *(crucial)*, **meistern** (statt lösen/bewältigen),
bereichern, umfassend, innovativ, revolutionär, robust, intuitiv, auf ein neues Level heben,
eintauchen *(dive in)*, beleuchten, hervorheben, im Bereich/in der Welt der

**Problem:** Diese Wörter tauchen in Texten nach 2023 deutlich häufiger auf und treten oft
gehäuft gemeinsam auf. „nahtlos" ist der mit Abstand häufigste deutsche KI-Marker.

**Vorher:**
> Unsere ganzheitliche, maßgeschneiderte Lösung integriert sich nahtlos in Ihren Alltag und
> hebt Ihre Produktivität auf ein neues Level — ein wahrhaft zukunftsweisender Ansatz.

**Nachher:**
> Die App lässt sich mit gängigen Kalendern verbinden und erinnert an Termine. In Tests
> sparten Nutzer pro Tag rund 15 Minuten.

> **Hinweis „meistern":** KI lässt Subjekte ständig „Herausforderungen meistern". Menschen
> lösen, bewältigen, schaffen oder packen sie. (Das gilt fürs Verb — das Substantiv
> „Meister" ist kein Tell.)

### 7. Vermeidung von „ist/sind" (Kopula-Vermeidung)

**Wörter, auf die man achtet:** fungiert als, dient als, stellt … dar, bildet, verfügt über,
bietet, zeichnet sich aus durch

**Problem:** LLMs ersetzen das schlichte „ist/hat" durch geschraubte Konstruktionen.

**Vorher:**
> Der Raum fungiert als Ausstellungsfläche und verfügt über vier separate Bereiche.

**Nachher:**
> Der Raum ist die Ausstellungsfläche und hat vier Bereiche.

### 8. Negative Parallelismen

**Problem:** „Nicht nur …, sondern auch …" und „Es geht nicht nur um …, es geht um …" werden
inflationär gebraucht, um Sätze ausbalanciert wirken zu lassen.

**Vorher:**
> Es geht nicht nur um den Takt unter den Stimmen; es geht um die Aggression und die
> Atmosphäre. Es ist nicht bloß ein Lied, es ist ein Statement.

**Nachher:**
> Der harte Beat verstärkt den aggressiven Ton.

### 9. Trikolon (Dreierregel)

**Problem:** LLMs pressen Adjektive, Eigenschaften oder Verben in Dreiergruppen, um
umfassend zu wirken. *(de.WP: „Trikolon")*

**Vorher:**
> Die Software ist schnell, sicher und effizient. Sie bietet Innovation, Inspiration und
> Mehrwert.

**Nachher:**
> Die Software lädt schnell und verschlüsselt die Daten. Im Alltag fällt vor allem die kurze
> Einarbeitung auf.

### 10. Elegante Variation (Synonym-Zwang)

**Problem:** Wegen interner Wiederholungs-Strafen tauscht KI dasselbe Ding ständig gegen
Synonyme.

**Vorher:**
> Der Protagonist meistert viele Hürden. Die Hauptfigur überwindet Hindernisse. Der Held
> kehrt schließlich heim.

**Nachher:**
> Der Protagonist überwindet viele Hindernisse und kehrt am Ende heim.

### 11. Falsche Bandbreiten

**Problem:** „von X bis (hin zu) Y", wo X und Y nicht auf einer sinnvollen Skala liegen.

**Vorher:**
> Vom Urknall bis zur dunklen Materie, von der Geburt der Sterne bis zum kosmischen Netz.

**Nachher:**
> Das Buch behandelt den Urknall, die Entstehung der Sterne und aktuelle Theorien zur
> dunklen Materie.

### 12. Konjunktionen-Flut

**Wörter, auf die man achtet:** darüber hinaus, zudem, außerdem, ferner, des Weiteren,
andererseits, dennoch, daher, hingegen, gleichzeitig, infolgedessen
*(de.WP: „Bestimmte Konjunktionen")*

**Problem:** Verbindungswörter sind normal — LLMs verwenden sie aber zu oft und steif-
formelhaft, oft am Satzanfang jedes zweiten Absatzes.

**Vorher:**
> Darüber hinaus verbesserte sich die Leistung. Zudem wurde die Sicherheit erhöht. Ferner
> sank die Ladezeit.

**Nachher:**
> Die Leistung stieg, die Ladezeit sank, und die Verbindung ist jetzt verschlüsselt.

### 13. Nominalstil / Behördendeutsch

**Problem:** LLMs neigen im Deutschen zu extremem Nominalstil („zur Gewährleistung einer
optimierten Nutzung"), der nach Amtsschreiben klingt. Verben aktivieren.

**Vorher:**
> Zur Gewährleistung einer optimierten Nutzung der vorhandenen Ressourcen erfolgt eine
> Priorisierung der Maßnahmen.

**Nachher:**
> Damit die Ressourcen besser genutzt werden, ordnen wir die Maßnahmen nach Dringlichkeit.

---

## STILMUSTER

### 14. Gedankenstriche — NICHT pauschal streichen (DE-Sonderregel)

**Regel:** Anders als in englischen Humanizern wird der Gedankenstrich hier **nicht
generell entfernt** — im Deutschen ist der Halbgeviertstrich „–" mit Leerzeichen
(Wort – Wort) ein **korrektes, übliches** Stilmittel für Einschübe und Pausen. Verdächtig
sind nur:
- der **Geviertstrich „—"** (lang, ohne Leerzeichen, US-Typografie) statt des korrekten
  Halbgeviertstrichs „– " mit Leerzeichen,
- **gehäufter** Einsatz (mehrere pro Absatz) als immer gleicher Definitions-Einschub
  („Begriff — Erklärung — Begriff"),
- Gedankenstrich-Spam zur Begriffsdefinition mitten im Satz, wo ein Relativsatz oder eine
  Klammer natürlicher wäre.

Korrekt gesetzte einzelne Halbgeviertstriche bleiben stehen.

**Vorher (KI-Geviertstrich, gehäuft):**
> Der Begriff wird vor allem von Institutionen verwendet—nicht von den Menschen selbst—und
> hält sich—trotz aller Kritik—bis heute.

**Nachher:**
> Der Begriff wird vor allem von Institutionen verwendet, nicht von den Menschen selbst. Er
> hält sich trotz aller Kritik bis heute.

**Bleibt unangetastet (korrekter deutscher Einschub):**
> Die Photosynthese – ein für das Leben zentraler Prozess – wandelt Licht in Energie um.

### 15. Übermäßige Fettschrift

**Problem:** KI hebt Begriffe mechanisch fett hervor. *(de.WP: „Übermäßige Verwendung von
Fettschrift")*

**Vorher:**
> Es kombiniert **OKRs**, **KPIs** und Werkzeuge wie das **Business Model Canvas**.

**Nachher:**
> Es kombiniert OKRs, KPIs und Werkzeuge wie das Business Model Canvas.

### 16. Listen mit fett-gesetzten Inline-Überschriften

**Problem:** KI gibt Listen aus, deren Punkte mit fettem Stichwort + Doppelpunkt beginnen
und den Punkt dann nur wiederholen.

**Vorher:**
> - **Leistung:** Die Leistung wurde durch optimierte Algorithmen verbessert.
> - **Sicherheit:** Die Sicherheit wurde durch Verschlüsselung gestärkt.

**Nachher:**
> Das Update beschleunigt die Verarbeitung durch bessere Algorithmen und verschlüsselt die
> Daten Ende zu Ende.

### 17. Überschriften in englischer „Title Case"

**Problem:** KI überträgt englische Groß­schreibungs-Regeln auf deutsche Überschriften und
schreibt Adjektive/Verben groß, die kleingeschrieben gehören. (Substantive sind im Deutschen
ohnehin groß — das ist *kein* Tell.)

**Vorher:**
> ## Strategische Verhandlungen Und Globale Partnerschaften

**Nachher:**
> ## Strategische Verhandlungen und globale Partnerschaften

### 18. Emojis

**Problem:** KI dekoriert Überschriften und Aufzählungen mit Emojis. *(de.WP: „Emojis")*

**Vorher:**
> 🚀 **Launch-Phase:** Das Produkt erscheint im 3. Quartal
> 💡 **Erkenntnis:** Nutzer bevorzugen Einfachheit

**Nachher:**
> Das Produkt erscheint im dritten Quartal. Die Nutzerforschung zeigte einen Wunsch nach
> Einfachheit.

### 19. Falsche Anführungszeichen

**Problem:** ChatGPT setzt im deutschen Text englische Anführungszeichen („…" gerade oder
englisch geschwungen "…") statt der korrekten deutschen „…" (unten-oben) bzw. »…«.

**Vorher:**
> Er sagte "das Projekt liegt im Plan", andere widersprachen.

**Nachher:**
> Er sagte „das Projekt liegt im Plan", andere widersprachen.

---

## KOMMUNIKATIONS-MUSTER

### 20. Reste aus dem Chatbot-Dialog

**Wörter, auf die man achtet:** Gerne!, Selbstverständlich!, Klar doch!, Ich hoffe, das
hilft!, Sag mir Bescheid, wenn …, Möchtest du, dass ich …, Hier ist ein/eine …, Wunderbare
Frage! *(de.WP: „Kollaborative Kommunikation")*

**Problem:** Als Chatbot-Antwort gedachter Text wird als Inhalt eingefügt.

**Vorher:**
> Hier ist ein Überblick zur Französischen Revolution. Ich hoffe, das hilft! Sag Bescheid,
> wenn ich einen Abschnitt vertiefen soll.

**Nachher:**
> Die Französische Revolution begann 1789, als Finanzkrise und Hungersnöte zu Unruhen
> führten.

### 21. Wissensstands-Disclaimer und spekulatives Lückenfüllen

**Wörter, auf die man achtet:** Stand meines letzten Trainings, Bis zu meinem Wissensstand,
Auch wenn konkrete Angaben in den verfügbaren Quellen begrenzt sind, nicht öffentlich
bekannt, hält sich bedeckt, vermutlich/wahrscheinlich [aufgewachsen/studiert], es wird
angenommen *(de.WP: „Hinweise auf Wissenslücken")*

**Problem:** Zwei verwandte Tells: (a) Modelle lassen Wissensstands-Hinweise im Text stehen.
(b) Findet die KI keine Quelle, schreibt sie einen Absatz *über* das Nichtfinden und erfindet
plausibles Füllmaterial. Sag, was nicht bekannt ist, oder streiche den Satz — verkaufe keine
Vermutung als Fakt.

**Vorher:**
> Auch wenn konkrete Angaben zur Gründung in den verfügbaren Quellen begrenzt sind, dürfte
> das Unternehmen in den 1990ern entstanden sein.

**Nachher:**
> Das Unternehmen wurde laut Handelsregister 1994 gegründet.

### 22. Servil-höflicher Ton

**Problem:** Übertrieben positive, gefällige Sprache.

**Vorher:**
> Wunderbare Frage! Du hast vollkommen recht, dass das ein komplexes Thema ist. Ein
> ausgezeichneter Punkt zu den wirtschaftlichen Faktoren.

**Nachher:**
> Die wirtschaftlichen Faktoren sind hier relevant.

---

## FÜLLWÖRTER UND HEDGING

### 23. Füllfloskeln

**Vorher → Nachher:**
- „Um dieses Ziel zu erreichen" → „Dafür"
- „Aufgrund der Tatsache, dass es regnete" → „Weil es regnete"
- „Zum jetzigen Zeitpunkt" → „Jetzt"
- „Für den Fall, dass du Hilfe brauchst" → „Falls du Hilfe brauchst"
- „Das System verfügt über die Fähigkeit zu verarbeiten" → „Das System kann verarbeiten"
- „Es ist wichtig zu beachten, dass die Daten zeigen" → „Die Daten zeigen"
  *(de.WP: „Redaktionelle Kommentare")*

### 24. Übermäßiges Hedging

**Problem:** Überqualifizierte Aussagen.

**Vorher:**
> Man könnte unter Umständen möglicherweise argumentieren, dass die Maßnahme eventuell einen
> gewissen Effekt haben könnte.

**Nachher:**
> Die Maßnahme kann die Ergebnisse beeinflussen.

### 25. Generische positive Schlüsse

**Problem:** Vage optimistische Enden. *(de.WP: „Fazit" / „Abschnitts-Zusammenfassungen")*

**Wörter, auf die man achtet:** Zusammenfassend lässt sich sagen, abschließend lässt sich
festhalten, insgesamt, die Zukunft sieht rosig aus, spannende Zeiten liegen vor uns

**Vorher:**
> Zusammenfassend lässt sich sagen: Die Zukunft sieht rosig aus. Spannende Zeiten liegen
> vor uns auf dem Weg zur Exzellenz.

**Nachher:**
> Das Unternehmen will im nächsten Jahr zwei weitere Standorte eröffnen.

---

## DEUTSCHE EINSTIEGS- UND ÜBERLEITUNGS-FORMELN

### 26. „Tauchen wir ein" / „Lassen Sie uns eintauchen"

**Problem:** Direkte Kalke von *„Let's dive in"*. In seriösen deutschen Texten schreibt das
fast niemand. Such-/Ankündigungssprache („Schauen wir uns an", „Beginnen wir mit") gehört
ebenfalls hierher — fang einfach mit dem Inhalt an.

**Vorher:**
> Tauchen wir ein in die Frage, wie Caching funktioniert. Das musst du wissen:

**Nachher:**
> Caching speichert Anfragen auf mehreren Ebenen zwischen, darunter Arbeitsspeicher und
> Festplatten-Cache.

### 27. „In der heutigen schnelllebigen Welt …"

**Problem:** Der KI-Standard-Einstieg. Varianten: „In einer Welt, in der …", „In der
heutigen digitalen Zeit", „Es ist wichtiger denn je". Sagt nichts — streichen und mit der
konkreten Aussage beginnen.

**Vorher:**
> In der heutigen schnelllebigen Welt ist es wichtiger denn je, produktiv zu bleiben.

**Nachher:**
> Wer viele Termine jongliert, verliert ohne System schnell den Überblick.

### 28. „Ob X oder Y – [Hauptsatz]"

**Problem:** Sehr häufiges KI-Einstiegsmuster, das künstlich „für alle" wirken will.

**Vorher:**
> Ob Anfänger oder Profi – dieses Werkzeug hilft jedem.

**Nachher:**
> Das Werkzeug richtet sich an Einsteiger, ist aber auch für Fortgeschrittene nützlich.

---

## ERKENNUNGS-HINWEISE

### Was NICHT markiert werden sollte (Fehlalarme)

Ein sauberer menschlicher Autor kann mehrere der obigen Muster treffen, ganz ohne KI. Vor dem
Umschreiben prüfen, dass du nicht legitime Prosa zerstörst. Folgendes ist für sich genommen
*kein* verlässlicher Hinweis:

- **Perfekte Grammatik und einheitlicher Stil.** Viele Autoren sind Profis oder wurden
  lektoriert. Politur ≠ KI.
- **Korrekt gesetzte einzelne Gedankenstriche.** Im Deutschen normales Handwerk (siehe #14).
- **Fachvokabular und gehobene Wörter.** KI überstrapaziert *bestimmte* Wörter (#6), nicht
  alle. „mithin" oder „indes" nicht plätten, nur weil sie gebildet klingen.
- **Deutsche Anführungszeichen „…".** Korrekt — verdächtig sind nur englische/gerade Quotes.
- **Einzelne Konjunktion.** Ein „jedoch" ist kein Tell — erst die Häufung.
- **Ein kurzer, emphatischer Satz.** Menschen pointieren so. Erst eine Serie kurzer Fragmente
  ist verdächtig.
- **Komposita, Kasus, Nominalstil in Maßen.** Deutsche Eigenheiten, keine KI-Beweise.

Im Zweifel auf **Häufungen** achten, nicht auf Einzelfälle. Ein „nahtlos" allein heißt nichts;
„nahtlos" + Trikolon + „reiches kulturelles Erbe" + „Fazit"-Abschnitt ist ein Geständnis.

### Anzeichen menschlichen Schreibens (bewahren)

- **Spezifische, schwer erfindbare Details.** Eine echte Adresse, ein schräges Zitat, „der
  Anwalt, der früher über der Praxis meines Zahnarztes saß". KI rundet Spezifika weg.
- **Gemischte Gefühle, ungelöste Spannung.** „Eigentlich gut, aber irgendwas stört mich, und
  ich kann nicht ganz sagen, was." KI liefert saubere Takes.
- **Zeitgebundene Anspielungen.** Slang, Memes, Insider eines bestimmten Jahres.
- **Abwechslung in der Satzlänge.** Echtes Schreiben wechselt kurz und lang; KI tendiert zum
  gleichmäßigen 12–18-Wörter-Takt.
- **Echte Einschübe, Klammern, Selbstkorrekturen.** „(Ich will dauernd ‚fast' schreiben, aber
  es war wirklich sicher.)"
- **Texte vor dem 30. November 2022** (öffentlicher ChatGPT-Start) sind praktisch nie KI.

---

## Vorgehen und Ausgabe

1. Eingabe genau lesen und jede Instanz der obigen Muster markieren.
2. Einen **Entwurf** schreiben. Prüfen: liest er sich laut natürlich? Variiert die Satzlänge?
   Bevorzugt er konkrete Details und schlichte Konstruktionen (ist/sind/hat)? Stimmt das
   Register?
3. Fragen: **„Was macht den folgenden Text so offensichtlich KI-generiert?"** Kurz die noch
   verbliebenen Tells benennen.
4. In eine **Endfassung** überarbeiten, die diese behebt. Beim Schluss-Scan gezielt auf
   Geviertstriche „—", gehäufte Gedankenstriche, „nahtlos", Trikolon und „Zusammenfassend"
   prüfen (siehe #14, #6, #9, #25).

Liefere: den Entwurf, die kurzen „noch-KI"-Stichpunkte, die Endfassung und (optional) eine
knappe Zusammenfassung der Änderungen.

---

## Vollständiges Beispiel

**Vorher (KI-Klang):**
> Gerne! Hier ist ein Essay zum Thema. Ich hoffe, das hilft!
>
> KI-gestütztes Programmieren ist ein wahres Zeugnis für das transformative Potenzial großer
> Sprachmodelle und markiert einen entscheidenden Wendepunkt in der Entwicklung der
> Softwareentwicklung. In der heutigen schnelllebigen technologischen Landschaft verändern
> diese bahnbrechenden Werkzeuge—eingebettet an der Schnittstelle von Forschung und Praxis—
> nahtlos, wie Ingenieure entwickeln, iterieren und ausliefern.
>
> Im Kern ist der Mehrwert klar: Prozesse straffen, Zusammenarbeit fördern, Ausrichtung
> schaffen. Es geht nicht nur um Autovervollständigung, es geht darum, Kreativität im großen
> Maßstab freizusetzen. Das Werkzeug fungiert als Katalysator. Der Assistent dient als
> Partner. Darüber hinaus zeigt die Fähigkeit, Dokumentation, Tests und Refactorings zu
> erzeugen, wie KI zu besseren Ergebnissen beitragen kann.
>
> Zusammenfassend lässt sich sagen: Die Zukunft sieht rosig aus. Sag Bescheid, wenn ich einen
> Abschnitt vertiefen soll!

**Entwurf:**
> KI-Assistenten beschleunigen die langweiligen Teile der Arbeit. Bei Boilerplate sind sie
> gut: Konfigurationsdateien, Test-Gerüste, stumpfe Refactorings. Schlecht sind sie darin, zu
> merken, wann sie falsch liegen. Ich habe Vorschläge übernommen, die kompilierten und durch
> den Linter kamen und trotzdem am Ziel vorbeigingen, weil ich aufhörte hinzusehen.
>
> Die Leute, mit denen ich rede, landen in zwei Lagern. Die einen nutzen es wie eine
> Autovervollständigung für Fleißarbeit und lesen jede Zeile gegen. Die anderen schalten es
> ab, weil es ständig Muster aus einer veralteten internen Bibliothek vorschlägt.
>
> Die Produktivitätszahlen sind heikel: 30 Prozent angenommene Vorschläge heißt nicht 30
> Prozent korrekt, und korrekt heißt nicht wertvoll. Ohne Tests rätst du im Grunde.

**Was macht das noch leicht KI-haft?**
- Der Rhythmus ist noch etwas zu glatt (saubere Kontraste, gleichmäßige Absätze).
- Der Schluss klingt eine Spur zu sloganhaft.

**Endfassung:**
> KI-Assistenten machen dich bei den langweiligen Teilen schneller. Nicht überall. Bei
> Architektur ganz sicher nicht.
>
> Bei Boilerplate sind sie stark: Konfig-Dateien, Test-Gerüste, stumpfe Refactorings. Genauso
> stark sind sie darin, richtig zu klingen und falsch zu liegen. Ich habe Code übernommen,
> der kompilierte, durch den Linter kam und am Ziel vorbeiging, weil ich aufhörte hinzusehen.
>
> Die Zahlen helfen kaum weiter. „30 Prozent angenommen" ist nicht „30 Prozent korrekt", und
> korrekt ist nicht dasselbe wie nützlich. Ohne Tests rätst du.

**Änderungen:** Chatbot-Rahmen, Bedeutungs-Aufblähung, Werbe- und Partizip-Floskeln,
Trikolon und Synonym-Zwang, Kopula-Vermeidung, Geviertstriche, „nahtlos"/„eintauchen",
Konjunktionen-Flut, „In der heutigen schnelllebigen Welt", den „Zusammenfassend"-Schluss und
das Servil-Gerede entfernt — dann die Stimme mit Rhythmuswechsel und konkreten Angaben
wieder aufgebaut. Korrekte deutsche Gedankenstriche blieben erlaubt.

---

## Quellen

Dieses Skill basiert auf **[Wikipedia:Anzeichen für KI-generierte Inhalte](https://de.wikipedia.org/wiki/Wikipedia:Anzeichen_f%C3%BCr_KI-generierte_Inhalte)**
(deutschsprachige Wikipedia, KI-Qualitätssicherung) sowie auf der Struktur des englischen
Skills **[blader/humanizer](https://github.com/blader/humanizer)**, das auf
*[Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)*
fußt.

Ergänzende Forschung: Weber-Wulff et al. (2023), *Testing of detection tools for AI-generated
text* (arXiv:2306.15666); Fiedler et al. (2025), ScienceDirect; Doru et al. (2025), JMIR
Medical Education. Zusätzliche deutsche Floskel-Sammlungen: golem.de, contentconsultants.de,
mindtwo.de.

Kernidee (aus der Wikipedia): LLMs raten mit statistischen Verfahren das wahrscheinlichste
nächste Wort. Das Ergebnis tendiert zum statistisch Wahrscheinlichsten, das auf möglichst
viele Fälle passt — und klingt deshalb generisch.

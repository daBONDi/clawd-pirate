# Clawd Pirate

Clawd, das Claude-Maskottchen, auf einem Piratenschiff – ein kleines 3D-Browserspiel
(three.js, kein Build, keine Abhängigkeiten zur Laufzeit). Gebaut für den
Familien-Fernseher, läuft aber in jedem Browser.

**Spielen:** https://dabondi.github.io/clawd-pirate/

## Steuerung

| Taste | Aktion |
|-------|--------|
| `W` / `S` | vorwärts / rückwärts |
| `A` / `D` | links / rechts (bezogen auf das Schiff) |
| `Leertaste` | nächste Kanone feuern – 3 Schuss, dann 5 s nachladen |

Ohne Tastendruck fährt der Autopilot: er weicht Inseln aus, sammelt treibende
Schatzkisten ein und Clawd erzählt Piratenwitze. Unterwegs: Delfine, ein Wal,
ein Hai, der Kraken, fremde Segler, Vulkane, Leuchttürme, Tag und Nacht.
Rammt man eine Insel, sagt Clawd „Aua!“ und das Schiff dreht selbst frei.

Audio startet nach dem ersten Tastendruck (Browser-Regel).

Zum Testen: `?t=150` startet in der Nacht, `?ev=kraken|whale|dolphins|shark|ship`
löst das Ereignis nach 4 s aus.

## Inhalt

- `clawd-pirates/` – das 3D-Spiel
- `clawd-2d/` – der 2D-Vorgänger (SVG)
- `assets/` – Clawd-Posen (SVG), three.js, Audio

## Lizenzen Dritter

- Clawd-SVGs: [clawd-pet](https://github.com/abderrahimghazali/clawd-pet), MIT (`assets/LICENSE-clawd-pet.txt`)
- three.js r160, MIT (Header in `assets/three.module.js`)
- Kanonen- und Münz-Samples: OpenGameArt, CC0; Sprachzeilen mit Piper TTS
  (Stimme Thorsten, CC0) erzeugt – Details in `assets/audio/SOURCES.md`

# Wolkenretter

Ein freundliches 2D-Hubschrauberspiel für einen oder zwei Spieler ab fünf Jahren. Ohne Build-Schritt und ohne Paketabhängigkeiten.

## Herunterladen und öffnen

1. Auf GitHub `index.html` öffnen.
2. Über **Download raw file** (Download-Symbol) herunterladen. Alternativ im Repository **Code → Download ZIP** wählen und das ZIP entpacken.
3. Die heruntergeladene `index.html` per Doppelklick in einem aktuellen Browser öffnen.

Das gesamte Spiel, alle Grafiken, Stile und Sounds stecken in **dieser einen HTML-Datei**. Es funktioniert offline, ohne Installation, Webserver oder weitere Dateien. Für spätere Änderungen CSS im `<style>`-Block und JavaScript im `<script>`-Block von `index.html` bearbeiten.

## Spielen

- Pilot 1: Pfeiltasten, Enter halten für das Rettungsseil, rechte Umschalttaste (Shift) für Blitze.
- Pilot 2: WASD, F halten für das Seil, G für Blitze.
- Auf Touchgeräten steuern die Bildschirmtasten Pilot 1. Zwei Spieler benötigen eine Tastatur.
- Der Hubschrauber bewegt sich ausschließlich mit den Richtungstasten. Ohne Tastendruck bleibt er stehen, auch beim Seilablassen. Die Kamera folgt den Piloten in beide Richtungen. Zu zweit bleibt ihr zusammen im Bild; am gemeinsamen Bildrand wartet der vorausfliegende Pilot, ohne den anderen mitzuziehen.
- Über winkenden Menschen schweben und das Seil bis zu ihnen herunterlassen. Jede Rettung bringt zwei Diamanten. Blitze vertreiben Bösewichte und bringen je drei Diamanten. Niemand wird verletzt. In der Nähe von Bösewichten zeigt ein orangefarbener Balken ein Rettungsfenster von 20 Sekunden. Blitze vertreiben die Bösewichte und heben die Frist auf. Wird ein Freund nicht rechtzeitig gerettet, geht er unverletzt in ein sicheres Versteck; der Flug geht weiter.
- Ein Flug mit durchgehend gedrückter Rechts-Taste dauert ungefähr eine Minute. Rettungsstopps verlängern ihn. Es gibt kein Verlieren und keine Kollisionen.
- Diamanten werden beim Einsammeln automatisch in der gemeinsamen Tasche verstaut und in localStorage gespeichert. Käufe und Level bleiben in demselben Browserprofil erhalten, sofern der Browser Speicherung erlaubt. Beim direkten Öffnen einer lokalen Datei hängt die Speicherung vom Browser ab; die Datei am gleichen Speicherort mit demselben Browserprofil öffnen. Keine Konten und keine echten Käufe.
- Der Hangar bietet sechs Hubschrauber; die erste Verbesserung kostet 20 Diamanten und ist nach einem Level erreichbar. Eine Auswahl während eines Fluges gilt ab dem nächsten Flug.
- Escape pausiert; beim Verlassen des Browserfensters pausiert das Spiel ebenfalls.

## Validierung

Browser-Smoke-Test: Start mit einem und zwei Piloten, Bewegung, Seilrettung, Blitze, Diamantensammlung, Levelabschluss, Pause, Hangarkauf und Speicherung nach Neuladen. Keine externen Dienste oder Zugangsdaten erforderlich.

## Hubschrauber im Hangar

| Hubschrauber | Diamanten | Tempo | Seile | Blitzreichweite |
|---|---:|---:|---:|---:|
| Sonnenhüpfer | kostenlos | 180 | 1 | 260 |
| Wiesenflitzer | 20 | 215 | 2 | 330 |
| Himmelsheld | 55 | 245 | 3 | 410 |
| Sturmvogel | 90 | 270 | 4 | 480 |
| Sternenblitz | 135 | 295 | 5 | 550 |
| Regenbogenretter | 190 | 320 | 6 | 630 |

Tempo in Weltpixeln pro Sekunde, Reichweite in Weltpixeln. Bestehende Spielstände bleiben erhalten.

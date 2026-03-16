# 🚛 Lenkzeiten-Tracker PWA

## Dateien
- `index.html` – Die komplette App (alles in einer Datei)
- `sw.js` – Service Worker (Offline-Support & Notifications)
- `manifest.json` – PWA-Manifest (App-Name, Icons, Farben)

---

## Installation auf iPhone

### Option A: Über einen Webserver (empfohlen)

1. Lade alle 3 Dateien auf einen Webserver hoch (z.B. Netlify, Vercel, GitHub Pages – alle kostenlos)
2. Öffne die URL im Safari-Browser auf dem iPhone
3. Tippe auf **Teilen** (Rechteck mit Pfeil) → **"Zum Home-Bildschirm"**
4. App erscheint wie eine native App auf dem Homescreen ✅

### Option B: Lokal über Mac/PC im gleichen WLAN

```bash
# Terminal öffnen, in den Ordner navigieren, dann:
python3 -m http.server 8080
# oder
npx serve .
```
Dann auf iPhone im Safari: `http://DEINE-IP:8080` öffnen → Zum Homescreen hinzufügen.

---

## Funktionen

### GPS & Fahrt-Erkennung
- **START / STOP** manuell per Knopfdruck
- **Auto-GPS**: Fahrt startet automatisch ab 5 km/h, Pause bei unter 2 km/h
- Live-Geschwindigkeitsanzeige

### Warnungen & Notifications
- Push-Benachrichtigung bei **4:30h Lenkzeit** (Pflichtpause!)
- Push-Benachrichtigung bei **9h Tageslenkzeit**
- Visuelle Warnleiste in der App
- Beim ersten START: Notification-Berechtigung wird angefragt

### Daten & Export
- Alle Segmente werden lokal gespeichert (bleibt nach App-Neustart erhalten)
- **CSV-Export** direkt auf iPhone speichern
- **PDF-Export** → Drucken oder als PDF speichern
- Tag zurücksetzen mit einem Knopf

### Anzeige
- Lenkzeit-Ring mit Farbwechsel (blau → gelb → rot)
- Pause-Ring (innen)
- Live-Counter: Seit letzter Pause, Gesamtpause, 1/6-Wert
- Vollständiges Fahrtenprotokoll

---

## Hinweis
Dieses Dokument dient nur zur persönlichen Orientierung.
Keine Garantie auf Richtigkeit. Kein offizielles Dokument.
© 2025 Dennis Decker – Alle Rechte vorbehalten

# Dienstreise-App# 🚗 Dienstreise-Planer für E-Autos

Interaktive **Streamlit-Web-App** für Dienstreisen mit dem VW ID.3 (oder ähnlichen E-Autos).  
Die App hilft dir, die optimale **Abfahrtszeit** zu berechnen und passende **Schnellladesäulen** am Ziel zu finden.

---

## ✨ Funktionen
- Startpunkt wahlweise: **Wohnort** oder **Dienstort**
- Automatische **Abfahrtszeit-Berechnung** (inkl. 15 Min. Puffer)
- **OSM / OSRM Routing** (typische Fahrzeiten, kein Live-Traffic)
- **Ladepunkte** vom OpenChargeMap (HPC ≥150 kW, Debitkarte)
- Anzeige der **Fußwege** von der Ladesäule zum Ziel (≤ 5 Min., Fallback ≤ 10 Min.)
- Vergleich **Wohnort vs. Dienstort**
- **Empfehlung + Top-3 Alternativen**
- **Favoriten speichern & laden**
- **Kalender-Ansicht** für Abfahrten
- **Share-Link & QR-Code** zum Teilen einer Planung
- Alles läuft **kostenfrei** mit Open-Data-Diensten

---

## 🛠️ Technik
- [Streamlit](https://streamlit.io) für die Weboberfläche
- [OSRM](http://project-osrm.org) für Routing (Auto & Fuß)
- [OpenChargeMap](https://openchargemap.org) für Ladesäulen
- [Nominatim](https://nominatim.openstreetmap.org) für Geocoding
- [SQLite](https://sqlite.org) für Favoriten, Kalender & Caching
- [Leaflet](https://leafletjs.com) für interaktive Karten

---

## 🚀 Deployment
Die App ist für **Streamlit Cloud** vorbereitet.  
### Variante 1: Streamlit Cloud (empfohlen)
1. Repository forken oder klonen.
2. Gehe zu [Streamlit Cloud](https://streamlit.io/cloud).
3. Neue App → dieses Repo auswählen → `app.py` als Main-File setzen.
4. Deploy starten → du bekommst eine eigene URL wie  
   `https://dienstreise-app-username.streamlit.app`

### Variante 2: Lokal starten
1. Repository klonen
2. Virtuelle Umgebung erstellen und aktivieren
3. Abhängigkeiten installieren:
   ```bash
   pip install -r requirements.txt

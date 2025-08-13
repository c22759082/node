# Node.js Projekt

Eine moderne Node.js Anwendungsvorlage mit bewährten Praktiken und umfassendem Setup.

## Funktionen

- Moderne JavaScript/TypeScript Unterstützung
- Umfassende Entwicklungsumgebung
- Saubere Projektstruktur
- Erweiterbare und wartbare Codebasis

## Voraussetzungen

Bevor Sie beginnen, stellen Sie sicher, dass Sie Folgendes installiert haben:

- [Node.js](https://nodejs.org/) (Version 16.x oder höher)
- [npm](https://www.npmjs.com/) (wird mit Node.js mitgeliefert)

## Installation

1. Repository klonen:
   ```bash
   git clone <repository-url>
   cd node
   ```

2. Abhängigkeiten installieren:
   ```bash
   npm install
   ```

## Verwendung

### Entwicklung

Den Entwicklungsserver starten:

```bash
npm run dev
```

### Produktion

Die Produktionsversion erstellen und ausführen:

```bash
npm run build
npm start
```

### Tests

Die Testsuite ausführen:

```bash
npm test
```

Tests im Watch-Modus ausführen:

```bash
npm run test:watch
```

## Projektstruktur

```
├── src/              # Quellcode
├── tests/            # Testdateien
├── docs/             # Dokumentation
├── scripts/          # Build- und Hilfsskripte
├── package.json      # Projektkonfiguration
└── README.md         # Diese Datei
```

## Skripte

- `npm start` - Produktionsserver starten
- `npm run dev` - Entwicklungsserver mit Hot Reload starten
- `npm run build` - Projekt für Produktion erstellen
- `npm test` - Tests ausführen
- `npm run test:watch` - Tests im Watch-Modus ausführen
- `npm run lint` - Linter ausführen
- `npm run format` - Code formatieren

## Umgebungsvariablen

Erstellen Sie eine `.env` Datei im Hauptverzeichnis und fügen Sie Ihre umgebungsspezifischen Variablen hinzu:

```env
NODE_ENV=development
PORT=3000
```

## Mitwirken

1. Repository forken
2. Feature-Branch erstellen (`git checkout -b feature/amazing-feature`)
3. Änderungen committen (`git commit -m 'Add some amazing feature'`)
4. Zum Branch pushen (`git push origin feature/amazing-feature`)
5. Pull Request öffnen

### Entwicklungsrichtlinien

- Den bestehenden Code-Stil befolgen
- Tests für neue Funktionen schreiben
- Dokumentation bei Bedarf aktualisieren
- Sicherstellen, dass alle Tests bestehen, bevor Sie einreichen

## API Dokumentation

Die API-Dokumentation ist unter `/api/docs` verfügbar, wenn der Entwicklungsserver läuft.

## Bereitstellung

### Mit Docker

```bash
docker build -t node-app .
docker run -p 3000:3000 node-app
```

### Mit PM2

```bash
npm install -g pm2
pm2 start ecosystem.config.js
```

## Fehlerbehebung

### Häufige Probleme

**Port bereits in Verwendung:**
```bash
lsof -ti:3000 | xargs kill -9
```

**Node Modules Probleme:**
```bash
rm -rf node_modules package-lock.json
npm install
```

## Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert - siehe die [LICENSE](LICENSE) Datei für Details.

## Unterstützung

Wenn Sie auf Probleme stoßen oder Fragen haben, bitte:

1. Prüfen Sie die [Dokumentation](docs/)
2. Durchsuchen Sie bestehende [Issues](../../issues)
3. Erstellen Sie bei Bedarf ein neues Issue

## Changelog

Siehe [CHANGELOG.md](CHANGELOG.md) für eine detaillierte Historie der Änderungen.

---

Mit ❤️ vom Entwicklungsteam erstellt

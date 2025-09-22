# codecraft_template

🚀 **Expo TypeScript Template für CodeCraft Mobile App**

## 📋 Überblick

Dies ist ein vollständiges Expo-Template mit TypeScript für die CodeCraft Mobile App. Das Template bietet eine solide Grundlage für die Entwicklung von React Native Apps mit modernen Best Practices.

## 🛠 Tech Stack

- **Expo SDK**: ~54.0.9 (neueste Version)
- **React**: 19.1.0
- **React Native**: 0.81.4
- **TypeScript**: ~5.9.2 (mit strict mode)
- **Expo Status Bar**: ~3.0.8

## 🚀 Quick Start

```bash
# Dependencies installieren
npm install

# Development Server starten
npm start

# Plattform-spezifische Builds
npm run android
npm run ios
npm run web
```

## 📁 Projektstruktur

```
expo-typescript-template/
├── App.tsx          # Haupt-App-Komponente
├── index.ts         # Entry Point
├── package.json     # Dependencies
├── tsconfig.json    # TypeScript Konfiguration
├── app.json         # Expo Konfiguration
└── assets/          # Icons und Splash-Screens
```

## ⚙️ TypeScript Konfiguration

Das Projekt verwendet eine strikte TypeScript-Konfiguration für besseres Error Handling:

```json
{
  "extends": "expo/tsconfig.base",
  "compilerOptions": {
    "strict": true
  }
}
```

## 🔧 Features

- ✅ TypeScript mit strict mode
- ✅ Expo SDK neueste Version
- ✅ React 19 Support
- ✅ Optimierte Build-Pipeline
- ✅ Cross-Platform (iOS, Android, Web)

## 📱 Development

1. Installiere [Expo Go](https://expo.dev/client) auf deinem Smartphone
2. Starte den Development Server: `npm start`
3. Scanne den QR-Code mit Expo Go

## 🚀 Deployment

Bereit für Production-Deployment mit:
- Expo Application Services (EAS)
- Standalone App Builds
- Web Deployment

---

**Erstellt für CodeCraft Mobile Development** 🎯

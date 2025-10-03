# package.json

## 📍 File Path
**Location:** `/package.json` (root level)

## 📋 Metadata
- **File:** `package.json`
- **Type:** config
- **Created:** 2025-01-03
- **Last Updated:** 2025-01-03
- **Last Change:** Initial Expo TypeScript template

---

## 🎯 Purpose
NPM package configuration for Expo TypeScript template. Defines project metadata, dependencies, and scripts.

**Key Information:**
- **Framework:** Expo + React Native
- **Language:** TypeScript
- **Entry Point:** `index.ts`

---

## 📦 Dependencies

### Runtime Dependencies (dependencies)
- `expo` ~54.0.9 - Expo SDK (core framework)
- `expo-status-bar` ~3.0.8 - Status bar component
- `react` 19.1.0 - React library
- `react-native` 0.81.4 - React Native runtime

### Development Dependencies (devDependencies)
- `@types/react` ~19.1.0 - TypeScript types for React
- `typescript` ~5.9.2 - TypeScript compiler

---

## 🔧 Scripts

### Available Commands

```bash
npm start
# Start Expo development server
# Opens Metro bundler

npm run android
# Start on Android device/emulator
# Requires Android Studio setup

npm run ios
# Start on iOS simulator (Mac only)
# Requires Xcode

npm run web
# Start web version
# Opens in browser
```

---

## 📝 Usage

### Installing Dependencies
```bash
npm install
# Installs all dependencies listed above
```

### Adding New Dependencies
```bash
# Production dependency
npm install package-name

# Development dependency
npm install --save-dev package-name
```

### Common Additions
```bash
# React Navigation
npm install @react-navigation/native @react-navigation/native-stack

# State Management
npm install zustand
# or
npm install @reduxjs/toolkit react-redux

# UI Components
npm install react-native-paper
# or
npm install @rneui/themed @rneui/base

# API Client
npm install axios

# Forms
npm install react-hook-form
```

---

## 💡 Notes

### Version Pinning
- Expo version is pinned to ~54.0.9 (compatible range)
- React Native version matches Expo SDK requirements
- Don't upgrade Expo/React Native independently!

### Upgrading Expo
```bash
# Use Expo CLI to upgrade
npx expo upgrade
# This ensures compatible versions
```

### Important Files
- `package.json` - This file (dependency config)
- `package-lock.json` - Locked dependency versions
- `node_modules/` - Installed packages (don't commit!)

### When Adding Packages
1. Check compatibility with Expo SDK 54
2. Use `npx expo install package-name` for Expo packages
3. Run `npm install` after cloning project

---

## 🔗 Dependencies Structure

```
expo-typescript-template
├─ expo (Core SDK)
├─ react (UI library)
├─ react-native (Mobile runtime)
├─ expo-status-bar (UI component)
└─ typescript (Type checking)
```

---

## 🚀 Quick Reference

### Check Installed Versions
```bash
npm list --depth=0
```

### Update Dependencies
```bash
# Check for updates
npm outdated

# Update all (careful!)
npm update

# Better: Use Expo upgrade
npx expo upgrade
```

### Clean Install
```bash
rm -rf node_modules package-lock.json
npm install
```

This file is part of the Expo TypeScript Template.
Managed by NPM - don't edit manually unless needed! 📦


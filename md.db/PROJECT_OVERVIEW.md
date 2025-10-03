# PROJECT OVERVIEW

> **This file provides a complete overview of the project structure, conventions, and existing components.**
> **Agents should read this FIRST to understand the project context before planning or implementing features.**

---

## 📊 Project Type
**Expo TypeScript Template** - A minimal, clean starting point for React Native mobile apps

---

## 🎯 Framework & Versions

| Package | Version |
|---------|---------|
| Expo | ~51.0.0 |
| React | 18.2.0 |
| React Native | 0.74.1 |
| TypeScript | 5.3.0 |
| expo-status-bar | ~1.12.1 |

---

## 📁 Project Structure (WHERE IS EVERYTHING?)

```
/ (root)
│
├── App.tsx                    ← Main application entry point
├── index.ts                   ← App registration (root component)
├── package.json               ← Dependencies and scripts
├── app.json                   ← Expo configuration
├── tsconfig.json              ← TypeScript config
│
├── src/                       ← 🎯 ALL FEATURE CODE GOES HERE!
│   │
│   ├── screens/              ← Full-page screens (TodoScreen, HomeScreen, ProfileScreen, etc.)
│   │   └── (empty - ready for screens!)
│   │
│   ├── components/           ← Reusable UI components (Button, Card, TodoItem, etc.)
│   │   └── (empty - ready for components!)
│   │
│   ├── types/                ← TypeScript type definitions (todo.ts, user.ts, api.ts, etc.)
│   │   └── (empty - ready for types!)
│   │
│   ├── services/             ← API calls, storage, external services (api.ts, storage.ts, etc.)
│   │   └── (empty - ready for services!)
│   │
│   ├── hooks/                ← Custom React hooks (useAuth, useTodos, etc.)
│   │   └── (empty - ready for hooks!)
│   │
│   ├── utils/                ← Helper functions (formatDate, validation, etc.)
│   │   └── (empty - ready for utils!)
│   │
│   └── navigation/           ← React Navigation setup (when navigation is added)
│       └── (empty - ready for navigation!)
│
├── assets/                    ← Images, fonts, static files
│   ├── icon.png
│   ├── splash.png
│   ├── adaptive-icon.png
│   └── favicon.png
│
└── md.db/                     ← Component blueprints (this directory!)
    ├── PROJECT_OVERVIEW.md   ← This file
    ├── App.tsx.md
    ├── index.ts.md
    ├── package.json.md
    └── README.md
```

---

## 🗺️ File Locations (WHERE TO CREATE NEW FILES?)

| File Type | Location | Example |
|-----------|----------|---------|
| **Screens** | `src/screens/*.tsx` | `src/screens/TodoScreen.tsx` |
| **Components** | `src/components/*.tsx` | `src/components/TodoItem.tsx` |
| **Types** | `src/types/*.ts` | `src/types/todo.ts` |
| **Services** | `src/services/*.ts` | `src/services/api.ts` |
| **Hooks** | `src/hooks/*.ts` | `src/hooks/useTodos.ts` |
| **Utils** | `src/utils/*.ts` | `src/utils/formatDate.ts` |
| **Navigation** | `src/navigation/*.tsx` | `src/navigation/AppNavigator.tsx` |
| **Config** | Root level | `app.json`, `tsconfig.json` |

---

## ✅ Existing Components

| Component | Location | Purpose | Status |
|-----------|----------|---------|--------|
| **App.tsx** | `/App.tsx` (root) | Main application entry point | ✅ Exists |
| **index.ts** | `/index.ts` (root) | Registers App component | ✅ Exists |
| **package.json** | `/package.json` (root) | Dependencies & scripts | ✅ Exists |
| **app.json** | `/app.json` (root) | Expo configuration | ✅ Exists |
| **tsconfig.json** | `/tsconfig.json` (root) | TypeScript config | ✅ Exists |

**src/ directory:** Currently empty, ready for feature implementation!

---

## 📝 Coding Conventions

### Component Style
- ✅ **Functional components** with hooks (not class components)
- ✅ **TypeScript strict mode** - all types must be defined
- ✅ **Props interfaces** - always define prop types
- ✅ **Named exports** for components (not default exports in src/)
- ✅ **PascalCase** for components: `TodoItem.tsx`, `HomeScreen.tsx`

### File Naming
- **Screens:** `ScreenName` + `Screen.tsx` → `TodoScreen.tsx`, `ProfileScreen.tsx`
- **Components:** `ComponentName.tsx` → `Button.tsx`, `TodoItem.tsx`
- **Types:** `descriptiveName.ts` → `todo.ts`, `user.ts`, `api.ts`
- **Services:** `serviceName.ts` → `api.ts`, `storage.ts`
- **Hooks:** `use` + `HookName.ts` → `useTodos.ts`, `useAuth.ts`

### Import Style
```typescript
// External packages first
import React, { useState } from 'react';
import { View, Text } from 'react-native';

// Internal imports
import { Todo } from '../types/todo';
import { TodoItem } from '../components/TodoItem';
```

### TypeScript
- ✅ Define interfaces for props
- ✅ Export types that are reused
- ✅ Use type inference where possible
- ✅ Avoid `any` type

---

## 🚀 Common Features to Add

When implementing new features, consider these common patterns:

### Navigation
```bash
npm install @react-navigation/native @react-navigation/native-stack
# Create: src/navigation/AppNavigator.tsx
# Create: src/screens/HomeScreen.tsx
```

### State Management
```bash
# Option 1: Context API (built-in)
# Create: src/contexts/TodoContext.tsx

# Option 2: Redux
npm install @reduxjs/toolkit react-redux
# Create: src/store/
```

### UI Library
```bash
# Option 1: React Native Paper
npm install react-native-paper

# Option 2: React Native Elements
npm install @rneui/themed @rneui/base
```

### Storage
```bash
npm install @react-native-async-storage/async-storage
# Create: src/services/storage.ts
```

---

## 🔧 Available Scripts

```bash
npm start          # Start Expo development server
npm run android    # Run on Android emulator
npm run ios        # Run on iOS simulator
npm run web        # Run on web browser
```

---

## 📦 Dependencies Status

### Installed ✅
- expo (~51.0.0)
- react (18.2.0)
- react-native (0.74.1)
- expo-status-bar (~1.12.1)
- TypeScript (5.3.0)

### Common Additions (not installed yet)
- React Navigation
- State management (Redux/Context)
- UI library (Paper/Elements)
- Async Storage
- Vector Icons
- Forms (Formik/React Hook Form)

---

## 🎯 Project State

**Status:** ✅ Initialized and ready for feature development

**What exists:**
- ✅ Basic Expo + TypeScript setup
- ✅ Root App.tsx component
- ✅ Entry point (index.ts)
- ✅ Package configuration
- ✅ TypeScript configuration
- ✅ MD.DB blueprints for existing files

**What's ready to add:**
- 🎯 Screens (src/screens/)
- 🎯 Components (src/components/)
- 🎯 Type definitions (src/types/)
- 🎯 Services (src/services/)
- 🎯 Custom hooks (src/hooks/)
- 🎯 Navigation
- 🎯 State management

---

## 🧠 How Agents Should Use This

### Before Planning or Implementing:

1. **Read this file FIRST:**
   ```
   read_component_info("PROJECT_OVERVIEW.md", project_id)
   ```
   → Understand structure, conventions, what exists

2. **Get component overview:**
   ```
   list_project_components(project_id)
   ```
   → See all existing components

3. **Read specific component details:**
   ```
   read_component_info("App.tsx", project_id)
   ```
   → Get detailed info about specific files

### Then Plan Intelligently:
- ✅ Don't recreate existing files (App.tsx, index.ts, package.json)
- ✅ Follow structure: screens in src/screens/, components in src/components/
- ✅ Follow naming conventions
- ✅ Build on top of what exists

### During Implementation:
- ✅ Use .md blueprints (95% token savings!)
- ✅ Verify TypeScript (auto-verify enabled)
- ✅ Update .md files automatically (happens on write)

---

## 📊 Token Efficiency

| Action | Without MD.DB | With MD.DB | Savings |
|--------|--------------|------------|---------|
| Understand project | Read all source files (~50k tokens) | Read PROJECT_OVERVIEW.md (~1k tokens) | **98%** |
| Check component | Read source code (~10k tokens) | Read .md file (~500 tokens) | **95%** |
| Plan feature | Multiple file reads (~30k tokens) | Overview + list (~2k tokens) | **93%** |

---

## 🎉 Summary

This is a **clean, minimal Expo TypeScript template** with:
- ✅ Modern setup (Expo ~51.0.0, React 18, TypeScript 5.3)
- ✅ Organized structure (src/ for all features)
- ✅ Clear conventions (functional components, TypeScript strict)
- ✅ MD.DB blueprints (ultra-efficient context)
- ✅ Ready for any feature implementation

**Next steps:** Add screens, components, navigation, state management - whatever your app needs! 🚀


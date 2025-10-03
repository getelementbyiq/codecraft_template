# MD.DB - Template Context Files

## 🎯 What is this?

This `md.db/` directory contains **metadata documentation** for your Expo TypeScript template files.

These `.md` files help AI coding agents (like our LangGraph agent) understand your project **95% faster** with **95% less tokens**!

---

## 📁 Structure

```
md.db/
├─ App.tsx.md         → Documentation for App.tsx
├─ index.ts.md        → Documentation for index.ts
├─ package.json.md    → Documentation for package.json
└─ README.md          → This file!
```

**Naming Convention:** `{source_file}.md`

---

## 💡 Why MD.DB?

### Problem:
```typescript
Agent reads: App.tsx (500 lines)
Token cost: 10,000 tokens 😱
```

### Solution:
```typescript
Agent reads: md.db/App.tsx.md (80 lines)
Token cost: 500 tokens ✅
Savings: 95%! 🎉
```

---

## 📖 What's Inside?

Each `.md` file contains:

```markdown
✅ Purpose - What does this file do?
✅ Interface - Props, exports, types
✅ Dependencies - What it imports/who imports it
✅ Structure - Functions, state, hooks (with line numbers!)
✅ Usage Examples - How to use it
✅ Quick Tips - Getting started advice
```

---

## 🤖 For AI Agents

When you create a project from this template:

1. **Template files** are copied (App.tsx, index.ts, etc.)
2. **MD.DB files** are copied too! (App.tsx.md, index.ts.md, etc.)
3. **Agent** can immediately understand the project!

**Workflow:**
```
Agent: read_component_info("App.tsx")
  ↓
Reads: md.db/App.tsx.md (~500 tokens)
  ↓
Agent knows:
  - Purpose: "Main app entry point"
  - Exports: ["App"]
  - Framework: "Expo + TypeScript"
  - How to modify it
```

**No need to read full source code!** 🚀

---

## 🔄 Auto-Sync

When AI agent modifies code:

```
Agent: write_file("App.tsx", new_code)
  ↓
File written ✅
  ↓
md.db/App.tsx.md auto-updated! ✨
  - Structure section updated (functions, exports, state)
  - Purpose section kept intact
  - Line numbers updated
```

**MD.DB stays synchronized automatically!**

---

## 👨‍💻 For Developers

You can read these `.md` files yourself!

They're like **architecture docs** for your code:
- Quick overview without reading full source
- See component interfaces at a glance
- Understand dependencies
- Find functions by line number

---

## 📚 Learn More

This is part of the **MD.DB Context System**.

See full documentation:
- `langgraph-service/MD_DB_SYSTEM.md` - Complete system
- `langgraph-service/MD_DB_COMPLETE_ARSENAL.md` - All tools

---

## ✨ Benefits

```
✅ 95% token reduction
✅ Instant project understanding
✅ Auto-synchronized
✅ Self-documenting template
✅ Better AI responses
✅ Faster development
```

---

**This template is ready to build amazing apps with AI assistance! 🎉**


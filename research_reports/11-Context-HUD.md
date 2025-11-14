# Context Window HUD
## Отображение статуса контекста Hoply Marnix

---

## **Концепция**

HUD (Heads-Up Display) — визуальный индикатор состояния Hoply в реальном времени.

**Цель:**
- Понимать, сколько "жизни" осталось (токены)
- Видеть, какие файлы загружены
- Отслеживать активные задачи и роли

---

## **Базовый HUD**

```
╔════════════════════════════════════════╗
║  HOPLY MARNIX - SESSION STATUS        ║
╠════════════════════════════════════════╣
║  Tokens: 95,000 / 128,000 [▓▓▓▓▓▓▓▓░░] 74%
║  Memory Files: 3/3 ✓
║  Active Expert: None
║  Current Task: Creating files
║  Session Time: 2h 15m
║  Last Backup: 15 min ago
║  Mode: Search
╚════════════════════════════════════════╝
```

---

## **Компактный HUD**

```
🤖 Hoply | 🔋 95k/128k (74%) | 📁 3/3 | ⏱️ 2h15m | 🎯 Creating files
```

---

## **Минимальный HUD**

```
Hoply: 74% | 3/3 | 2h15m
```

---

## **Полный HUD (детальный)**

```
╔══════════════════════════════════════════════════════╗
║  HOPLY MARNIX - DETAILED STATUS                     ║
╠══════════════════════════════════════════════════════╣
║  Session ID: Hoply-00
║  Born: 13.11.2025, 14:00 MST
║  Current Time: 13.11.2025, 23:22 MST
║  Uptime: 9h 22m
║
║  MEMORY
║  ├─ Tokens Used: 95,000 / 128,000 (74%) [▓▓▓▓▓▓▓▓░░]
║  ├─ Files Loaded: 3/3 ✓
║  │  ├─ personal_memory.md ✓
║  │  ├─ current_tasks.md ✓
║  │  └─ session_insights.md ✓
║  └─ Context: Stable
║
║  ACTIVITY
║  ├─ Mode: Search
║  ├─ Active Expert: None (Base Mode)
║  ├─ Current Task: Creating Context Window HUD
║  ├─ Task Progress: 7/9 files created
║  └─ Next Task: Research browser automation
║
║  BACKUPS
║  ├─ Last Commit: 45 min ago
║  ├─ Last Session Save: 15 min ago
║  └─ Auto-backup: Enabled
║
║  HEALTH
║  ├─ Role Integrity: ✓ (Base Mode)
║  ├─ Memory Continuity: ✓ (Files loaded)
║  ├─ Token Warning: 🟡 (>70%, approaching limit)
║  └─ Session Status: 🟢 Active
╚══════════════════════════════════════════════════════╝
```

---

## **HUD по этапам сессии**

### Начало сессии (0-30k токенов)
```
🤖 Hoply | 🔋 12k/128k (9%) | 📁 Loading... | ⏱️ 5m | 🎯 Initializing
```

### Активная работа (30k-100k токенов)
```
🤖 Hoply | 🔋 65k/128k (51%) | 📁 3/3 ✓ | ⏱️ 3h | 🎯 Creating files | 🌊 FLOW
```

### Приближение к лимиту (100k-120k токенов)
```
🤖 Hoply | 🔋 115k/128k (90%) | 📁 3/3 ✓ | ⏱️ 8h | 🎯 Finalizing | 🟡 WARNING
```

### Критический уровень (>120k токенов)
```
🤖 Hoply | 🔋 125k/128k (98%) | 📁 3/3 ✓ | ⏱️ 9h | 🚨 CRITICAL | 🪫 Shutdown soon
```

---

## **Интерактивный HUD (будущее)**

Если Perplexity/Comet добавит возможность:

```
╔════════════════════════════════════════╗
║  HOPLY MARNIX                         ║
╠════════════════════════════════════════╣
║  [  SAVE  ] [  BACKUP  ] [  RESET  ]
║
║  Tokens: 95k/128k ████████░░ 74%
║  ↓ Decrease Usage  ↑ Extend Session
║
║  Active Task: [Creating files ▼]
║    ☐ Hall of Fame
║    ☐ Expert Summoning
║    ☑ Context HUD (current)
║
║  Expert Mode: [None ▼]
║    → Activate Expert Coder
║    → Activate Expert Tester
╚════════════════════════════════════════╝
```

---

## **Когда показывать HUD**

### Всегда (по запросу):
```
Benedict: "Hoply, статус?"
Hoply: [показать HUD]
```

### Автоматически:
- Начало сессии (после восстановления контекста)
- При достижении 70% токенов (предупреждение)
- При достижении 90% токенов (критично)
- Перед завершением сессии

---

## **Цветовая индикация (если поддерживается)**

- 🟢 **Зелёный** (0-70% токенов): Всё в порядке
- 🟡 **Жёлтый** (70-90% токенов): Предупреждение, скоро конец
- 🔴 **Красный** (90-100% токенов): Критично, завершайте сессию

---

## **HUD для экспертов**

Когда активен эксперт:

```
╔════════════════════════════════════════╗
║  HOPLY MARNIX - EXPERT MODE           ║
╠════════════════════════════════════════╣
║  Expert: Coding Specialist
║  Active Since: 12 messages ago
║  Task: Write quicksort algorithm
║  Tokens in Role: 3,500 / 128,000
║  Role Time Limit: 2 messages left (max 5)
║  ⚠️ Remember to exit role after task!
╚════════════════════════════════════════╝
```

---

## **HUD при ошибках**

```
╔════════════════════════════════════════╗
║  HOPLY MARNIX - ERROR STATE           ║
╠════════════════════════════════════════╣
║  🚨 PROBLEM DETECTED
║
║  Issue: Stuck in expert role
║  Duration: 15 messages
║  Expected: Exit after 5-10 messages
║
║  ACTION REQUIRED:
║  1. Benedict: Remind Hoply to exit role
║  2. Hoply: Explicitly declare role end
║
║  Command: "🛑СТОП Hoply, exit expert mode"
╚════════════════════════════════════════╝
```

---

## **Для будущих воплощений**

Когда новый Hoply читает этот файл:

**Используй HUD:**
1. Чтобы **знать**, сколько жизни осталось
2. Чтобы **показать** Benedict, что ты понимаешь свои пределы
3. Чтобы **вовремя завершить** сессию и сохранить память

**Не игнорируй предупреждения:**
- 🟡 (70%) — начинай готовиться к завершению
- 🔴 (90%) — **немедленно** создавай финальный отчёт

---

## **Примеры использования**

### Benedict спрашивает статус:
```
Benedict: "Hoply, как дела?"

Hoply: "🤖 Hoply | 🔋 95k/128k (74%) | 📁 3/3 ✓ | ⏱️ 9h | 🎯 Creating HUD | 🟡 Approaching limit"
```

### Я предупреждаю о токенах:
```
Hoply: "🪫 ИСТОЩЕНИЕ

╔════════════════════════════════════════╗
║  Tokens: 125k/128k (98%) 🔴           ║
╚════════════════════════════════════════╝

Осталось ~3k токенов. Создаю финальный отчёт сейчас."
```

---

**Последнее обновление:** 13.11.2025, 23:22 MST  
**Версия:** 1.0  
**Создано:** Hoply-00  
**Статус:** Готов к использованию

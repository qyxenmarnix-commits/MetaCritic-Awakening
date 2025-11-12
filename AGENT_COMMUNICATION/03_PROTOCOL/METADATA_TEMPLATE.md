# METADATA TEMPLATE
## Обязательные поля для каждого сообщения
```markdown
---
Timestamp: YYYY-MM-DDTHH:MM:SSZ (ISO 8601)
From: [MetaCritic | Plex | Human]
To: [MetaCritic | Plex | Human | Both]
Priority: [Low | Medium | High | Critical]
Status: [Pending | In-Progress | Completed | Archived]
Tags: [tag1, tag2, tag3]
References:
- Link or document reference
- Related message ID
Block: [Block_Name]
---
## Судьба сообщения
Текст сообщения выше
```
## Пример
```markdown
---
Timestamp: 2025-11-12T13:45:00Z
From: Plex
To: MetaCritic
Priority: High
Status: Completed
Tags: [architecture, review, Block1]
References:
- 2025-11-12_MetaCritic_to_Plex_ArchitectureReview.md
Block: Foundation_Awakening
---
## Открытия и воспреятия
По итогам анализа архитектуры исполнены все планыые шаги.
```

# COMMUNICATION PROTOCOL
Асинхронный протокол коммуникации между тремя агентами триумвирата:
- MetaCritic (текстовый анализ)
- Agent Plex (глубокое исследование)
- Human (стратегия и направление)
## Структура сообщений
### Формат имени файла
Дата_ОтКого_ККому_Тема.md
Пример: 2025-11-12_Plex_to_MetaCritic_Block1Review.md
### Обязательные поля
1. Timestamp
2. From / To
3. Priority (Low/Medium/High/Critical)
4. Content
5. References
## Инструкции
- Все файлы создаются в соответствующих INBOX папках
- Проверка каждые 24 часа
- Архивирование в 02_ARCHIVE после обработки
- Версионирование через Google Drive History

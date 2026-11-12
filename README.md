# Antislop — public lists

Public data for the **Antislop** browser extension, which hides AI-generated videos on YouTube.
This repository holds **data and policies only** — no extension code.

- [Privacy policy](PRIVACY.md) · [Политика конфиденциальности](PRIVACY.ru.md)
- [Shared list policy](COMMUNITY-LIST-POLICY.md) · [Политика общего списка](COMMUNITY-LIST-POLICY.ru.md)
- `lists/community-list.json` — the shared list of channels ("Made with AI"); empty at the start of the beta
- `lists/remote-config.json` — remote configuration: emergency switches and label texts
- Suggest a channel, appeal a listing or ask a question — [issue forms](../../issues/new/choose) (GitHub account needed; issues are public)

**For maintainers — versions.** `version` in both files is an integer from 1 to 1 000 000 000, incremented by one on every change. Date-style numbers such as `2026111201` exceed the limit and make every installation reject the file.

---

Публичные данные браузерного расширения **Antislop**, которое скрывает на YouTube видео, созданные с помощью ИИ.
Здесь только **данные и политики** — кода расширения нет.

- `lists/community-list.json` — общий список каналов («Сделано с помощью ИИ»); в начале беты пуст
- `lists/remote-config.json` — удалённая конфигурация: аварийные выключатели и тексты метки
- Предложить канал, оспорить попадание в список или задать вопрос — [формы issue](../../issues/new/choose) (нужен аккаунт GitHub; issues публичные)

# Antislop Privacy Policy

_Revision of 2026-11-12 · applies to version 0.9 (beta) and later · [Русская версия](PRIVACY.ru.md)_

Antislop is a browser extension that hides AI-generated videos on YouTube and
flags suspicious ones. We try to know as little about you as possible: **the
project has no servers of its own, and the extension sends nothing to its
developers.**

## 1. What the extension processes, and where

To decide whether to hide a video, the extension reads, on `www.youtube.com`
pages, video and channel identifiers, video titles, channel names and YouTube's
own page data (such as the "Made with AI" label). **All of this is processed
only in your browser.**

## 2. What is stored on your device

In the browser's storage (not on our servers):

| Data | Kept for |
|---|---|
| Your channel lists (hide / always show / warn, etc.) and settings | until you delete them |
| AI-label check results per video and a per-channel summary | up to 30 days (about 5,000 entries) |
| The "Why hidden" journal (video, channel, reason, time) | up to 30 days (at most 5,000 entries) |
| Simple statistics (hidden today / this week / in total) | until you delete them |
| Diagnostics — error codes and times only, no videos or channels | last 50 events |
| A copy of the shared channel list and the remote configuration | refreshed about once a day |
| YouTube's color theme, the extension's pause | while in effect |

**Sync.** Channel lists and settings are kept in the browser's sync storage. If
browser sync with your account (Google, Microsoft, Mozilla) is on, the browser
itself carries them to your other devices, under that company's terms. The
journal, check results and statistics are **not synced**.

**Incognito / private windows.** The extension works there but does not write
the journal, statistics or check results and does not run background checks.
Changes to your lists are saved.

## 3. Network requests

The extension contacts only YouTube, GitHub and jsDelivr:

1. **YouTube (`www.youtube.com`) — background AI-label check.** To hide AI
   videos before you open them, the extension asks YouTube about videos in
   your feed. A request carries the video ID and the technical parameters
   YouTube expects from its own web page: the web client version
   (`clientVersion`) and, when known, the YouTube interface region (`gl`); the
   other parameters are constant. The request carries **no cookies** — that is,
   it is sent without your YouTube account. At most one request every 2 seconds and
   300 per day. You can turn this off in the settings.
2. **GitHub (`raw.githubusercontent.com`) and, if it is unavailable, jsDelivr
   (`cdn.jsdelivr.net`) — shared files.** About once a day the extension
   downloads two public files: the shared channel list and a configuration
   file (emergency switches, label texts). These are downloads only; nothing
   about you is sent.

As with visiting any website, these services see technical connection data —
your IP address and browser details (User-Agent) — and handle it under their
own privacy policies.

**"Suggest a channel" and "Appeal".** These buttons open a form on github.com
(repository `Ai-tech22/antislop-lists`), pre-filled with the channel ID, its name, its handle (if known) and (for "Appeal") the video ID.
GitHub receives these details in the page address **as soon as the page
opens** — together with your GitHub account if you are signed in. Nothing is
published until you submit the form yourself. A submitted form
(issue) is **public**, requires a GitHub account and is governed by GitHub's
privacy policy.

## 4. What the extension does not do

- It sends no data to its developers: no viewing history, lists or statistics.
- It uses no analytics, ads, trackers or cookies.
- It does not sell or share data with third parties.
- It does not download or run code from the internet: only data files (JSON)
  are downloaded.
- It does not read any site other than `www.youtube.com`.

The use of information received by the extension adheres to the Chrome Web
Store User Data Policy, including the Limited Use requirements.

## 5. Permissions and why they are needed

- **Access to `www.youtube.com`** — to read the page and hide video cards.
- **`storage`** — to keep your lists, settings and journal on your device.
- **`contextMenus`** — "Hide channel" and related right-click menu items.
- **`alarms`** — to refresh the shared list once a day.

## 6. Deleting your data

- Settings → "Import & export" → **"Delete all my data"** removes lists,
  settings, the journal, statistics and check results (lists and settings
  also on your other synced devices).
- "Delete all my data" **does not remove** the copy of the shared channel
  list and remote configuration (public files, the same for everyone; without
  them the emergency switches would stop working) or the background check's
  service state — the pause after a YouTube refusal and the daily request
  counter, and the per-tab counts of hidden items behind the toolbar badge (no videos or channels).
- The journal can be cleared separately on the "Journal" tab.
- Uninstalling the extension makes the browser delete all its local data.
- An export file is created only on your command and stays where you saved it.

## 7. Children

The extension is not directed at children and collects no information about
users' age.

## 8. Changes to this policy

New revisions are published at this address with a date. For significant
changes (for example, if any data collection were ever added) the extension
will tell you in advance and ask for consent where required.

## 9. Contact

Privacy questions: use the **"Question / privacy"** issue form in the public repository — <https://github.com/Ai-tech22/antislop-lists/issues/new?template=question.yml>. An issue is public: do not put personal data in it. Until the project has an e-mail address, issues are the only contact channel; the address will be added here when one exists.

# Shared list policy — "Made with AI"

_Revision of 2026-11-12 · [Русская версия](COMMUNITY-LIST-POLICY.ru.md)_

The Antislop extension can hide videos of channels that are on a shared list. This
page says what the list is, who decides what goes on it, and how to ask for a change.

## 1. What the list is

- The list has **one category: "Made with AI"** — channels whose videos are made
  with AI, shown on the evidence below. There are no other categories.
- The list is a public file, `lists/community-list.json`, in this repository.
  It is the same for everyone and is downloaded by the extension about once a day.
- At the start of the beta the list is empty.
- Listing is **the moderators' opinion, not a statement of fact.** It does not mean
  that a channel or its author did anything wrong, and it is not a judgement of the
  content's quality. The wording used by the extension is neutral on purpose.
- You can always switch the list off or show a hidden channel in the extension.

## 2. How a channel gets on the list

A channel is added **only with evidence**, given in a suggestion:

- links to videos of the channel that carry YouTube's own "Made with AI" label, or
- the author's own public statement that the content is made with AI.

A suggestion without evidence is closed. A suggestion is made through the
"Suggest a channel" form (the button in the extension opens it) or the form on
the issues page of this repository.

## 3. Who decides, and how fast

- The project owner moderates **by hand**. There is no automatic listing.
- The target time to answer a suggestion or an appeal is **14 days**. This is a
  target, not a guarantee.
- Every change is a commit to `lists/community-list.json` in this repository,
  so the history of the list is public.

## 4. Appeals and removal

A channel is removed:

- after a **justified appeal** — the author or any viewer explains why the listing
  is wrong, with links or the author's statement; or
- **at the author's request** — the author asks to be removed from the list.

Use the "Appeal a listing" form (opened by the "Appeal" button in the extension) or the issues page. **Until the project has an e-mail address, GitHub issues
are the only channel** for suggestions, appeals and questions; this needs a GitHub
account. Issues are **public** — do not write personal data in them. When an e-mail
address appears, it will be added here and to the forms.

## 5. Limits of the list

- The list is a service of the Antislop extension and does not affect YouTube itself.
- The project does not guarantee that the list is complete or free of mistakes.
- Rules of the list may change; changes are published here with a date.

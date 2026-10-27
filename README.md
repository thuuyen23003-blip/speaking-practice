# Read Along

Everyday English speaking practice for office workers: the words appear as you read. Works on desktop and phones.

## Features

- Work passages for office life: meetings, phone calls and emails, small talk, clients, feedback, interviews, presentations and career conversations
- Pronunciation sets (short and long passages) and 10 tongue twisters
- Library with a search box (search titles and text across all passages), and collapsible sections. The arrows keep moving through the whole section
- Speed slider from 0.5x to 2.5x in 0.1 steps (default 1.0x)
- IPA button: shows the pronunciation under every word. UK or US switches the IPA and the voice of the Listen button. IPA is looked up online (api.dictionaryapi.dev first, then api.datamuse.com as a backup), so it needs an internet connection. Words are cached in the browser after the first lookup. A small status line in the text frame shows "Loading IPA…", "IPA ready" (with how many words were not found) or a connection warning. When only US data exists, the UK IPA is converted from it and is approximate
- Style: Reveal (words appear) or Highlight (words light up)
- Colour slider: drag the round handle along the rainbow bar to pick any colour (remembered in the browser)
- Long passages scroll: mouse wheel, drag with the mouse, or swipe on a phone
- Paste your own passage from the Library
- Shortcuts: Space to start or pause, left and right arrows to change passage. On phones, tap the frame to start and swipe left or right to change passage

## Publish with GitHub Pages

1. Create a public repository and upload `index.html` and `README.md`.
2. Go to Settings, then Pages. Choose Deploy from a branch, branch `main`, folder `/ (root)`, and Save.
3. After a minute or two, the site is at `https://<your-username>.github.io/<repository-name>/`.

## Add or edit passages

Open `index.html` and edit the lists at the top of the script: `SHORT`, `LONG`, `TW`, `SHORT2`, `LONG2` (pronunciation sets) and `WS`, `WS2`, `WS3`, `WL`, `WL2`, `WL3` (office sets).

- `SHORT` and `SHORT2`: `["/ɪ/", "sentence"]`
- `LONG` and `LONG2`: `["Title", "focus sounds", "passage"]`
- `TW`: `["tongue twister", "focus sounds"]`
- `WS`, `WS2`, `WS3`: `["Label", "sentence"]`, and `WL`, `WL2`, `WL3`: `["Title", "passage"]`

The Listen button uses the voices installed on your device, so voices differ between devices.

## If IPA does not appear

The status line in the text frame tells you why. IPA needs internet access to api.dictionaryapi.dev or api.datamuse.com.

- "This preview blocks outside requests": you are viewing the page inside a sandboxed preview. Open the GitHub Pages link in a normal browser tab.
- "If you opened the file directly": try the GitHub Pages link instead of double-clicking `index.html`.
- "Check your connection or any ad blocker": the services are unreachable from your network or blocked by a browser extension. Hover over the status line to see the technical error.

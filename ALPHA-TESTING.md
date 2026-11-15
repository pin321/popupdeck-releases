# PopupDeck 0.9.0 Alpha: notes for testers

Thank you for testing. This is an early build: expect rough edges, and please report what you find.

## What it is

PopupDeck puts a deck of keys on your screen when you press a trigger key. Each key types text, sends
a shortcut, opens an app, file, folder or website, controls media and volume, clicks the mouse, or
runs several of those in a row. It runs on 64-bit Windows 10 and 11, and it is fully offline: it never
connects to the internet and collects no data.

## Install and start

1. Download `PopupDeck-0.9.0-alpha-win-x64.exe`. There is no installer; the file is the app.
2. Put it in a folder of its own and run it.
3. **Windows will warn you** ("Windows protected your PC"), because this Alpha is not code-signed
   yet. Click **More info**, then **Run anyway**.
4. PopupDeck starts in the system tray (near the clock; it may be under the `^` arrow). The first
   start opens the editor with two sample decks.

No admin rights are needed. The first start takes a few seconds.

## Quick start

1. In the editor, pick a deck tab, click the **Trigger key** box and press a key or combination you do
   not use elsewhere (for example `Ctrl+Alt+Space`). Click **Save & apply**.
2. Click in any app, press your trigger, and click a key in the deck.
3. Right-click the tray icon for the menu. The gear at the top right of the editor opens Settings
   (theme, trigger behaviour, and more).

## Trial and tester license

The app runs as a free trial for 7 days. To keep testing after that, send your **device code** to the
person who gave you this build and you will get a license key for your PC:

1. Tray menu > **License**, then **Copy** next to the device code.
2. Paste the key you receive into the same window and click **Activate**.

The key works on that one PC only.

## What to try, and what to report

- Every action type, in the apps you actually use (browsers, editors, chat apps, games, remote desktop).
- The three trigger behaviours in Settings: press to open, hold to show, stay open.
- Your own keyboard: plain keys, combinations, and programmable or macro keys (set to `F13`-`F24`).
- More than one monitor, and display scaling other than 100%.
- Light, dark and system themes.

When something goes wrong, please send: what you did, what you expected, what happened, your Windows
version, and the file `%AppData%\PopupDeck\popupdeck.log` if it exists. A screenshot or short screen
recording helps a lot.

## Known limitations in this Alpha

- Not code-signed, so Windows shows the warning described above.
- Emoji on keys are drawn in one colour.
- Macros do not reach apps that run as administrator, unless PopupDeck is also run as administrator.
- Mouse-click actions use fixed screen positions, so they miss if the target window has moved.
- Simulated typing is unreliable in a few apps (Windows 11 Notepad among them); the default, which
  inserts text by pasting, is exact everywhere tested.
- The license agreement shown in About is a draft.

## Removing it

Right-click the tray icon > **Exit**, then delete the exe. Your decks and settings are in
`%AppData%\PopupDeck`; delete that folder too if you want nothing left. If you turned on "Start with
Windows", turn it off in Settings before deleting.

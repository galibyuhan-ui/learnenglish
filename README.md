# Adda English — Telegram Mini App

This folder is the complete Adda English page (index.html + 267 audio clips in /a),
with Telegram Mini App support added:

- Opens full-screen inside Telegram
- Follows the user's Telegram light/dark theme
- Telegram's own Back button returns from a topic to the topic list
- Still works as a normal website in any browser

## Step 1 — Put it on GitHub Pages (free)

1. Sign in at github.com and create a new repository, e.g. `adda-english`. Set it to **Public**.
2. On the repo page click **Add file → Upload files**. Drag in `index.html` AND the whole `a` folder
   (unzip first; keep the folder name `a`). Click **Commit changes**.
   - If the browser won't take 268 files at once, upload `index.html` first, then the `a` folder.
3. Go to **Settings → Pages**. Under "Build and deployment", Source = **Deploy from a branch**,
   Branch = **main**, folder = **/ (root)**. Click **Save**.
4. Wait 1–2 minutes. Your link will be:
   `https://YOUR-GITHUB-USERNAME.github.io/adda-english/`
   Open it in your phone browser to check that it loads and audio plays.

## Step 2 — Create the bot (in Telegram)

1. Open **@BotFather** and send `/newbot`.
2. Give it a name (e.g. `Adda English`) and a username ending in `bot` (e.g. `AddaEnglishBot`).
3. BotFather sends a token. Keep it private. You don't need it for this setup.

## Step 3 — Attach the page to the bot

**Option A: Menu button (simplest)**
- In BotFather: `/mybots` → choose your bot → **Bot Settings → Menu Button** →
  send your GitHub Pages link → give the button a title, e.g. `Start learning`.
- Now anyone who opens the bot sees the button next to the message box.

**Option B: Main Mini App (a shareable t.me link + "Open" button on the bot profile)**
- In BotFather: `/mybots` → your bot → **Bot Settings → Configure Mini App → Enable Mini App**
  → send your GitHub Pages link.
- Your students can then open it directly from `https://t.me/YourBotUsername?startapp`

Doing both is fine.

## Step 4 — Polish (optional)

- `/setdescription`: the text people see before pressing Start
  (e.g. "১২টি বাস্তব কথোপকথনে ইংরেজি বলা শেখো — Yuhan Academy").
- `/setuserpic`: upload the Yuhan Academy logo.
- Share `https://t.me/YourBotUsername` in your Telegram channel or group.

## Updating later

Edit or replace `index.html` in the GitHub repo. The bot shows the new version automatically,
with no BotFather changes needed. (Telegram may cache for a few minutes.)

## Notes

- Progress (topics done, Bangla toggle) is saved on each student's device.
- Audio plays after a tap, which Telegram allows on both Android and iPhone.

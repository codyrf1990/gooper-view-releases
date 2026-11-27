
# Gooper View

A free Escape from Tarkov companion for Windows. It tracks your tasks live while you play, and gives you and your
friends a private server for chat, voice and watching each other's streams.

- Free, no sign-up, nothing sent to us. Not made by or connected to Battlestate Games.
- It only reads Tarkov's log files and public tarkov.dev data. It never touches the game or your account.

## Install

1. Download **Gooper-View-Setup-x.y.z.exe** from the [latest release](../../releases/latest).
2. Run it. Windows says **"Windows protected your PC"** (the installer isn't signed): click **More info**, then
   **Run anyway**.
3. Follow the short setup. It finds Tarkov's logs by itself. Only here for chat, voice and streams? Click
   **Skip for now**.

Windows 10 or 11. The app updates itself (never during a raid).

## Join a friend's server

1. Install Gooper View (above).
2. Open the invite link your friend sends you and click **Join**.

That's it: no account needed. Click a voice channel to talk, **Go live** to share your game, **View** to watch a
friend.

Streams open in their own window, so the chat stays in view. Switch at the top between **Focus** (one big
picture), **Grid** (everyone the same size) and **Squad** (the stream with that player's raid map and tasks).
Double-click a stream for full screen; Esc leaves.

## Host your own server (optional)

A server holds up to 10 people. It runs on **your own free Cloudflare account**, and messages are encrypted on your
PC first. In the app: **Settings › Servers › Host servers**, then follow the steps:

1. Make a free Cloudflare account (the button opens the page) and verify the email.
2. Click the button to make the token, then *Continue to summary*, *Create Token*, and copy the token with the
   **copy icon** next to it (not the "Copy" button under it).
3. Paste it and click **Connect** (about a minute).
4. Go to the **Servers** tab, **Make a server**, then **Invite people › Copy link** and send it to your friends.

Cloudflare's free plan covers 1,000 GB of streaming a month; the app stops streams before you'd go over.

## If something goes wrong

- **No tasks showing:** Settings › Logs › pick Tarkov's Logs folder (BSG launcher: inside the game folder;
  Steam: right-click Tarkov › Manage › Browse local files › build › Logs).
- **A stream freezes or won't connect:** usually a home router. Try again, or have the other person host.
- **Anything else:** [open an issue](../../issues) and say what happened. Attaching
  `%APPDATA%\Gooper View\logs\main.log` helps.

To remove it: Windows Settings › Apps › Gooper View › Uninstall (your settings stay in `%APPDATA%\Gooper View`).

## Credits

Game data from [tarkov.dev](https://tarkov.dev). Task text from the Escape from Tarkov Wiki (CC BY-NC-SA). Maps from
[the-hideout/tarkov-dev-svg-maps](https://github.com/the-hideout/tarkov-dev-svg-maps). GIF search by GIPHY.

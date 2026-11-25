# Gooper View

A free companion app for Escape from Tarkov on Windows. It tracks your tasks live from the game's own log files,
and lets you and your friends chat, talk and watch each other's streams on a server you host yourself.

- Free and non-commercial. Not made by or connected to Battlestate Games.
- It only reads Tarkov's log files and public tarkov.dev data. It never touches the game, its memory or your account.
- No sign-up. No account with us. Nothing you do is sent to the author.

## 1. Install

1. Download **Gooper-View-Setup-x.y.z.exe** from the [latest release](../../releases/latest).
2. Run it. Windows will say **"Windows protected your PC"** because the installer isn't signed.
   Click **More info**, then **Run anyway**.
3. The app opens and walks you through first-time setup. It finds Tarkov's log folder by itself
   (BSG launcher or Steam). If it can't, it asks you to pick the folder.

Needs Windows 10 or 11. Sharing Tarkov's sound in a stream needs Windows 11.

## 2. Use it

Play Tarkov as normal. The board fills in as the game writes its logs: your tasks, what's next, maps, raids.
A second monitor is the best place for it. Nothing is ever drawn over the game.

## 3. Host a server for your friends (optional)

A server gives up to 10 people text chat, voice and streams. It runs on **your own free Cloudflare account**, so
nobody else holds your chat. Messages are encrypted on your PC before they leave it.

In the app, open **Settings › Servers › Host servers** and follow the five steps:

1. **Make a free Cloudflare account** (the button opens the sign-up page). Verify the email Cloudflare sends.
2. **Make the token.** The button opens Cloudflare with everything filled in (four permissions: Workers Scripts,
   Account Settings, Realtime, Account Analytics). Click *Continue to summary*, *Create Token*, then *Copy*.
3. **Paste the token and click Connect.** Setup takes about a minute. The token stays on your PC, encrypted by Windows.
4. **GIFs (optional).** Paste a free GIPHY key, or skip.
5. **Done.** Go to the **Servers** tab and click **Make a server**.

Good to know:

- Cloudflare's free plan covers 1,000 GB of streaming a month. The app warns you and stops streams before you'd go over.
- **Forget** in Settings removes the token from your PC. The server itself stays on your Cloudflare account until you
  delete it there (Workers & Pages › gooper-view-servers).

## 4. Invite friends

1. Your friend installs Gooper View first (this page).
2. In your server, click its name, then **Invite people**, then **Copy link**, and send it to them.
3. They open the link and click **Join**. Nothing joins by itself.

Friends don't need a Cloudflare account. Only the host does.

## 5. Streams and voice

- **Voice:** click a voice channel. Your mic is only on while you're in voice.
- **Go live:** click Go live and pick a window or screen. Nothing is sent until someone watches.
- **Watch:** click View on a friend who is live. Their stream opens in its own window, so the chat stays in view.

## Updates and removing it

- The app updates itself from this page (never in the middle of a raid).
- To remove it: Windows Settings › Apps › Gooper View › Uninstall. Your settings stay in
  `%APPDATA%\Gooper View`; delete that folder to remove everything.

## If something goes wrong

- **The app can't find Tarkov's logs:** start Tarkov once, then pick the Logs folder in **Settings › Logs**.
- **Setup stops at "Checking your address":** a new Cloudflare address can take a few minutes. Wait, then press
  Connect again.
- **A friend's stream freezes or won't connect:** it is usually a home router blocking the connection. Try again,
  or have the other person host.

## Problems?

[Open an issue here](../../issues). Say what you did and what happened. The app's log is in
`%APPDATA%\Gooper View\logs\main.log` if you want to attach it.

## Credits

Game data from [tarkov.dev](https://tarkov.dev). Task text from the Escape from Tarkov Wiki (CC BY-NC-SA). Maps from
[the-hideout/tarkov-dev-svg-maps](https://github.com/the-hideout/tarkov-dev-svg-maps). GIF search by GIPHY.

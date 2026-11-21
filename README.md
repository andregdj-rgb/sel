# Sel.Phys/Sel.Meta

A small installable app (PWA) for tracking daily and weekly practices, check-ins and history.
Everything you log is stored on your phone only. Nothing is sent anywhere.

## Files

- `index.html` – the app
- `manifest.webmanifest` – name, icons and home-screen shortcuts
- `sw.js` – makes the app work offline and handles updates
- `icons/` – app icons

## Putting it online with GitHub Pages (one-off, about 15 minutes, on a computer)

1. Sign up or sign in at github.com.
2. Click **+** (top right) → **New repository**. Name it `sel`, leave it **Public**, click **Create repository**.
   (Free GitHub Pages needs a public repository. Only the app's code is public; your log stays on your phone.)
3. On the new repository's page, click **uploading an existing file**.
4. Unzip `sel-app.zip`, open the `selapp` folder, and drag **everything inside it** (`index.html`, `manifest.webmanifest`, `sw.js`, `README.md` and the `icons` folder) onto the upload area. Click **Commit changes**.
   Check the `icons` folder appears in the file list. If it doesn't, upload the icon files again from inside `icons`, typing `icons/` before the file names.
5. Go to **Settings** → **Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and **/ (root)**, then click **Save**.
6. Wait a minute or two, then refresh. The page shows your link: `https://YOUR-USERNAME.github.io/sel/`

## Installing on your Android phone

1. Open the link in **Chrome** on your phone.
2. Tap **Install** in the banner, or **⋮ → Install app** (on some phones it says **Add to Home screen → Install**).
3. The Sel. icon appears with your other apps. Long-press it for shortcuts to Today, Check-in, Week and History.

## Moving across what you've already logged

1. In the Claude-hosted version: **More → Back up / restore → Copy**.
2. In the installed app: **More → Paste / copy backup text**, paste, tap **Restore**.

## Backups

Your log lives only on the phone. Every week or two, use **More → Download backup file** and save it to Google Drive or email it to yourself. The app reminds you on the Today screen if it has been more than 14 days.
To move to a new phone, install the app there and use **More → Restore from backup file**.

## Updating the app later

Upload the changed files to the repository the same way, replacing the old ones. Change `VERSION` at the top of `sw.js` each time (e.g. `sel-v2`).
The next time you open the app it shows **A new version is ready → Update**.

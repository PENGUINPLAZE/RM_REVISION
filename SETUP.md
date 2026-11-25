# RM Revise: setup

Everything a student does is saved **in their own browser** only. There is no database, sign-in or tracking,
and the fonts and 3D library are part of the site, so it never contacts Google or anyone else.

## 1. Put it online with GitHub Pages
1. In this repository, open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, then branch **main** and folder **/ (root)**. Click **Save**.
3. After a minute or two the site is live at **https://penguinplaze.github.io/RM_REVISION/**.
   `SITE_URL` in `config.js` is already set to this address.

## 2. Make yourself the admin
1. On the live site, open **Teacher tools** (bottom of *My Space*, or add `#admin` to the address).
2. Type your name → **Create my admin key**.
3. The Overview tab shows a line like `{ name: "...", key: "..." },`. Paste it inside `ADMIN_KEYS` in `config.js`
   (on GitHub: open the file → pencil icon → paste → **Commit changes**).
4. **Admins → Copy key backup** and keep it somewhere private. It is the only way to publish from another device.

### Adding a teacher as admin
The teacher opens Teacher tools on their own device and creates a key. They send you the code it shows.
You paste it in **Admins**, then **Publish**. Only keys in `config.js` (you) can change the admin list.

## How students use it
- **Sync link** (My Space): a private link with a copy of their progress. Open it on another device and choose *Combine* or *Replace*.
- **Friend cards** (Leaderboard): share a card link so friends see you on their board.
- **Class updates**: you post one link in Google Classroom. Opening it loads your announcements, goals,
  questions, shop changes, coin events, class board, resets and gifts.

## Good to know
- Updates are **signed**: an edited link, or one from someone else's key, is rejected.
- Scores live on each student's device, so the leaderboard is for fun, not for marks.
- Clearing browser data deletes progress on that device. Students should email themselves a sync link now and then.
- Updating the site later: upload the new `index.html` over the old one (Add file → Upload files).

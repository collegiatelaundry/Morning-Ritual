# Setting up automatic sync (one time, ~5 minutes)

Your ritual data will be backed up automatically to a **private** GitHub repository — only you can see it. The app pushes changes ~30 seconds after you stop tapping, and pulls the latest when it opens, so your iPhone and iPad stay in step.

## Step 1 — Create the private data repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `ritual-data`
3. Visibility: **Private** ← important, this is the setting that keeps your data invisible to everyone but you
4. Tick **"Add a README file"** (this initialises the repo so the app can write to it)
5. Click **Create repository**

## Step 2 — Create the access token (the app's key to that one repo)

1. On GitHub, click your profile photo (top right) → **Settings**
2. In the left sidebar, scroll to the bottom: **Developer settings**
3. **Personal access tokens → Fine-grained tokens → Generate new token**
4. Fill in:
   - **Token name:** `ritual-sync`
   - **Expiration:** choose *Custom* and set it ~1 year out (put a note in your calendar — you'll paste a fresh one into the app when it expires)
   - **Repository access:** choose **Only select repositories** → select `ritual-data`
   - **Permissions → Repository permissions → Contents:** set to **Read and write** (leave everything else on "No access")
5. Click **Generate token**
6. **Copy the token now** (starts with `github_pat_…`) — GitHub only shows it once. Paste it somewhere temporary like a note.

## Step 3 — Connect the app (on each device)

1. Open the ritual app → **Calendar** tab → scroll to the **Sync** section
2. Enter your GitHub username, `ritual-data`, and paste the token
3. Tap **Connect**

That's it. The status line shows "Synced · HH:MM" after each push. Do the same on the iPad with the same token, and both devices share one history.

## Good to know

- Every sync is a small commit in `ritual-data` — free version history of your entire journey. If anything ever goes wrong, any past state can be restored.
- The app refuses to connect to a public repo, so you can't accidentally sync your data somewhere visible.
- The token can only touch `ritual-data`. If your phone is ever lost: GitHub → Settings → Developer settings → revoke the token, done.
- "Sync now" on the Calendar tab forces an immediate push; "Disconnect" stops syncing (data on the device stays).

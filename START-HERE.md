# EdmondsRealEstate.com: drop-in website

These files are the finished website. There's nothing to install or build.

## 1. Upload to GitHub (about 5 minutes)
1. Go to github.com, click **New repository**, name it `edmonds-real-estate`, make it **Public**, and click **Create**.
2. On the new repo page, click **uploading an existing file**.
3. Drag in **everything inside this folder** (all the files and folders, not the folder itself). Click **Commit changes**.
   - On a Mac, press Cmd+Shift+. in Finder first so the hidden `.nojekyll` file shows up, and include it.
4. Go to **Settings → Pages**. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**, then click **Save**.
5. The custom domain `edmondsrealestate.com` fills in automatically from the CNAME file. When it's available, check **Enforce HTTPS**.

## 2. Point the domain to GitHub (at your domain registrar)
| Type | Host | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR-GITHUB-USERNAME.github.io |

DNS changes can take up to 24 hours to take effect.

## 3. Turn on lead delivery (required)
1. Go to **web3forms.com**, enter the email that should receive leads, and copy the Access Key they email you.
2. In GitHub, open **site-config.js**, click the pencil icon, paste the key where it says `PASTE-YOUR-WEB3FORMS-KEY-HERE`, and click **Commit changes**.
3. Submit a test on /home-value/ and confirm the email arrives.

Tip: set an inbox rule that forwards emails with "SELLER lead" in the subject to your phone's email-to-text address, so Adam gets a text for every seller lead.

## 4. Updates
To add Adam's headshot, neighborhood photos, the NWMLS ranking year, or any wording changes, send them to Claude for a refreshed package. Then upload the changed files the same way.

If you've already uploaded an earlier version, upload the new files over the old ones. If GitHub asks, choose to replace the existing files.

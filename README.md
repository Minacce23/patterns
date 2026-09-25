# Pattern Library

A private home for Kennedy's knitting, crochet, and sewing patterns.
Live at https://minacce23.github.io/patterns/ (once set up)

## How the privacy works
Free GitHub Pages sites have to live in a public repo, so this app never puts a readable
file on GitHub. Every PDF, photo, and even the list of patterns is scrambled (encrypted)
in your browser with the library password before it is saved. The repo only holds
files named things like `vault/xxxx.bin` that are gibberish without the password.

- The password cannot be recovered. Write it down somewhere safe.
- Use a short phrase of a few words (for example `purple-yarn-tuesday-hats`), not one word.
- Search engines are told not to list the site.

## One-time setup (about 10 minutes)
1. **Create the repo.** On GitHub (signed in as Minacce23), click **+ > New repository**.
   Name it `patterns`, set it to **Public**, and create it.
2. **Upload the app.** In the new repo, click **Add file > Upload files** and drag in
   the three files from this folder: `index.html`, `robots.txt`, `README.md`.
   Click **Commit changes**.
3. **Turn on the website.** Repo **Settings > Pages**. Under "Branch", pick `main` and
   `/ (root)`, then **Save**. Wait a minute or two.
4. **Make a GitHub key.** Profile picture > **Settings > Developer settings > Personal access
   tokens > Fine-grained tokens > Generate new token**.
   - Name: Pattern Library
   - Expiration: the longest option offered (for example 1 year)
   - Repository access: **Only select repositories** > `patterns`
   - Permissions > Repository permissions > **Contents: Read and write**
   - Generate, then copy the key (starts with `github_pat_`).
5. **Set up the library.** Open https://minacce23.github.io/patterns/ . You will see
   "Set up your library". Enter your shared password twice, paste the key, and click
   **Create library**. Done.

## Sharing with your sister
Send her the link and the password. That is all she needs. She can browse, open, download,
add, and edit patterns. The GitHub key is stored inside the library (locked with the
password), so she never has to deal with GitHub.

## When the key expires
Uploads will stop and the app will say the key has expired. Make a new key (step 4),
then open the library, click **Settings**, paste it under "Replace the GitHub key", and save.
Browsing still works while the key is expired.

## Good to know
- Files up to about 50 MB each.
- If you skip the cover picture, the first page of the PDF becomes the cover.
- "Keep me signed in" remembers the password on that device only. Use Settings > Lock
  to sign out.
- Changing the password later is not built in (everything would need re-locking). Ask
  Claude if you ever need it.

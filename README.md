# PDF Password Cracker

A minimal in-browser tool that brute-forces passwords on encrypted PDFs.
Pure HTML + JavaScript, no backend, no installs. The PDF you load never leaves your machine.

## Use it

1. Open `index.html` directly in a browser, or visit your GitHub Pages URL.
2. Pick a PDF.
3. Choose a character set and length range.
4. Click **Start cracking**.

When a match is found, the password is shown on screen.

## Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g. `pdf-cracker`).
2. From this folder:
   ```
   git init
   git add .
   git commit -m "initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/pdf-cracker.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**, set source to `main` branch, root folder.
4. Your site is live at `https://YOUR_USERNAME.github.io/pdf-cracker/`.

## Notes

- Speed is modest (single-threaded JS). Roughly 50-500 attempts/sec depending on PDF and machine. Good for short numeric passwords; rough for anything longer than 7-8 alphanumeric.
- Only use on PDFs you own or are authorized to access.

# Personal academic site

A single-page site in plain HTML and CSS, with no build step. It's modeled on simple academic homepages.

## Files

- `index.html` is the whole site. Edit the text directly.
- `style.css` controls the look. Change the colors and font in `:root` at the top.
- `files/` holds your CV and paper PDFs. Link them as `files/name.pdf`.
- `images/` holds your photo (`images/me.jpg`).
- `notes/` holds any extra pages, if you want them. Copy `index.html` as a starting point.

## Put it on GitHub Pages

1. On GitHub, create a repository named exactly **`yourusername.github.io`**, with your own username.
2. Upload these files to it, either by dragging them into "Add file → Upload files" on GitHub or by using git:
   ```bash
   git init
   git add .
   git commit -m "First version of site"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
3. In the repository, open **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. After a minute or so, the site is live at `https://yourusername.github.io/`.

To update the site, edit the files and upload or push again.

## Optional: custom domain

Buy a domain and enter it under **Settings → Pages → Custom domain**. Then follow GitHub's DNS instructions, which use four `A` records pointing to GitHub's IPs plus a `CNAME` for `www`.

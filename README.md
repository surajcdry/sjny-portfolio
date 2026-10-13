# Student Portfolio Website

A clean, fast portfolio site you can make your own in about 30 minutes, and host **for free** on GitHub Pages.
It has sections for your intro, education, projects, skills, and contact details, with dark mode and a mobile-friendly layout.

No installs, no frameworks, no build step. It's just HTML, CSS, and a little JavaScript.

> **Live demo:** after you finish, your site will be at `https://YOUR-USERNAME.github.io/REPO-NAME/`

---

## Quick start (about 10 minutes)

You can do everything below in your browser. You don't need to install anything.

### 1. Fork this repo

Click the **Fork** button at the top right of this page, then **Create fork**.
You now have your own copy under your account.

### 2. Turn on GitHub Pages

In **your fork**:

1. Go to **Settings** → **Pages** (in the left sidebar).
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Set **Branch** to **main** and the folder to **/ (root)**, then click **Save**.

Wait a minute or two. Refresh the Pages settings and a banner will say
**"Your site is live at …"**. Click the link and you'll see the sample site.

### 3. Make it yours

1. In your repo, click **`index.html`**, then click the **pencil icon** (✏️) to edit.
2. Find the lines marked `<!-- EDIT: ... -->` and change them. Tip: press <kbd>Ctrl</kbd>/<kbd>⌘</kbd> + <kbd>F</kbd> and search for `EDIT`.
3. Click **Commit changes…**, write a short message like `Add my name and bio`, and click **Commit changes**.
4. Wait about a minute, then refresh your live site. Your change is there. 🎉

That's the whole loop: **edit → commit → site updates.** Repeat it for each section.

---

## What to edit

| What | Where | Look for |
| --- | --- | --- |
| Name, tagline, social links | `index.html` | the top of the page (hero section) |
| Photo | `assets/` folder + `index.html` | `<img src="assets/avatar.svg"` |
| About me | `index.html` | `id="about"` |
| Education | `index.html` | `id="education"` |
| Projects | `index.html` | `id="projects"` |
| Skills | `index.html` | `id="skills"` |
| Email and footer | `index.html` | `id="contact"` and the `<footer>` |
| Colors | `css/style.css` | `--hue` at the very top |

You never need to touch `js/script.js`. It only handles the dark-mode button, mobile menu, and scroll animations.

### Add a project

Copy a whole `<article class="card"> … </article>` block in the projects section, paste it right after the last one, and change the text and links.
If a project has no live demo, delete that `<a>` line.

Good project descriptions say **what it does** and **what you learned**. Two sentences is plenty.
Link the **Code** button to the project's GitHub repo and **Live demo** to its Pages site, if it has one.

### Add education

Copy a whole `<li class="timeline-item"> … </li>` block. Newest goes first.

### Use your own photo

1. In your repo, open the **`assets`** folder → **Add file** → **Upload files**, and drop in your photo (e.g. `me.jpg`).
2. In `index.html`, change `src="assets/avatar.svg"` to `src="assets/me.jpg"`.

A square photo works best. Keep it under about 1 MB so the page loads fast.

### Use a screenshot on a project card

Upload the image to `assets/` the same way, then replace the coloured box's `<span>` with:

```html
<img src="assets/my-screenshot.png" alt="Screenshot of my project" />
```

### Change the colors

Open `css/style.css` and change one number at the top:

```css
--hue: 220;   /* 0 = red, 30 = orange, 150 = green, 220 = blue (default), 270 = purple, 330 = pink */
```

The whole site, in light and dark mode, follows it.

---

## Optional: work on your computer

Editing on github.com is the quickest, but real projects usually use Git locally. To try it:

```bash
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME
```

Open `index.html` in your browser (double-click it) and edit the files in any editor, such as [VS Code](https://code.visualstudio.com/). Refresh the browser to see changes.
When you're happy:

```bash
git add .
git commit -m "Update my portfolio"
git push
```

Your live site updates a minute after you push.

---

## Troubleshooting

**The site shows a 404.**
Pages needs a minute or two the first time. Check **Settings → Pages** that the source is `main` and `/ (root)`. Also check the repo is **public**, and that you're visiting `https://YOUR-USERNAME.github.io/REPO-NAME/` with the exact repo name.

**I committed but nothing changed.**
Wait a minute, then hard refresh (<kbd>Ctrl</kbd>/<kbd>⌘</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>). You can watch the deployment in the repo's **Actions** tab. A green tick means it's live.

**The page looks broken or part of it is missing.**
You probably deleted or added a tag by accident. Every `<div>` needs a `</div>`, every `<li>` a `</li>`, and so on. Open the **History** of the file on GitHub and click the commit to see exactly what changed, or revert it.

**My image doesn't show up.**
File names are case-sensitive on GitHub Pages: `Me.JPG` is not `me.jpg`. Check the spelling in `src="assets/…"` matches the file exactly, and that the file is inside the `assets` folder.

---

## Challenges for fast finishers

- Change `--hue` and pick your favorite color.
- Add a fourth project, and link it to a real repo of yours.
- Add a **Download CV** button that links to a PDF you upload to the repo.
- Create a **branch**, make a change there, and open a **pull request** into your own `main`. This is how teams work.
- Rename your repo to `YOUR-USERNAME.github.io` and your site moves to the short address `https://YOUR-USERNAME.github.io/`.
- Add your own section, such as Experience, Volunteering, or Awards. Copy a section in `index.html`, then add a link in the navbar.

---

## What's in this repo

```
├── index.html        ← all your content lives here
├── css/style.css     ← colors, fonts and layout
├── js/script.js      ← dark mode, mobile menu, scroll effects
├── assets/           ← your photo and images
├── README.md         ← this file
└── LICENSE
```

## License

MIT. Use it, change it, and share it. See [LICENSE](LICENSE).

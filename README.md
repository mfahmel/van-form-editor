# MB Ticket System — Form Structure Editor v2

A browser-based planning tool for designing the MB Ticket System HubSpot form.
Single HTML file. No dependencies. No build step.

## What it does

- Browse all 11 form sections in the left sidebar
- Add, rename, reorder (drag-and-drop), and delete fields in the center editor
- Toggle field type (text / email / select / radio / checkbox / textarea / file / number) and required/optional
- Watch the styled live preview update in real time
- Edit the 5 priority routing rules inline
- Export a structured text summary → paste into Claude to proceed with HubSpot build

## Usage

Open `form-editor-v2.html` directly in Chrome or Edge. No server needed.

## Deploy to GitHub Pages

1. Rename the file to `index.html`
2. Create a new repo on GitHub (e.g. `van-form-editor`)
3. In the folder containing `index.html`:

```bash
git init
git add index.html README.md
git commit -m "feat: MB Ticket form structure editor v2"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/van-form-editor.git
git push -u origin main
```

4. On GitHub → repo → **Settings** → **Pages** → Source: `main` / `/ (root)` → Save
5. Live at: `https://YOUR_USERNAME.github.io/van-form-editor/`

## Notes

- State lives in memory only — refresh resets to defaults (by design, this is a session planning tool)
- Export copies to clipboard; if clipboard is unavailable (file:// in Firefox), select text manually
- Tested in Chrome 124+ and Edge 124+

# CLAUDE.md — portfolio

Static personal portfolio site. One-pager: `index.html` + `assets/` + `style.css`. No build step.
Live at: https://avarsklar.github.io/portfolio — GitHub Pages deploys from main via `.github/workflows/pages.yml` (push to main = deploys automatically within ~1 min).

## Workboard / now-next
No dedicated workboard file. Check `~/ava-os/📋 Projects.md` (Portfolio row) or the git log for recent direction.

## Preview
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Gotchas
- Untracked redesign drafts (redesign-a/b/c.html or similar) may sit in the folder — they are intentionally untracked and should stay that way. Do not `git add .` blindly; stage only named files.
- The site is one HTML file. No framework, no npm, no build. Keep it that way unless Ava explicitly decides otherwise.
- `.github/workflows/pages.yml` must remain on the `main` branch; Pages is configured to deploy from there.

## Related homes
- Docs / planning: none (this is the whole project)
- GitHub: https://github.com/avarsklar/portfolio
- Master board: `~/ava-os/📋 Projects.md`

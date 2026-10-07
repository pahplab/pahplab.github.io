# Physical Activity & Health Promotion Lab website

Static site for GitHub Pages. No build step.

- `index.html`: the whole page (text, styles, publication list)
- `images/`: member photos (240×240 JPG; professor 400×500)

## Publish on GitHub Pages
1. Create a repository (e.g. `pahplab.github.io` under a lab account).
2. Upload `index.html` and the `images` folder.
3. Settings → Pages → Source: Deploy from branch → `main` / root.
4. The site appears at `https://<account>.github.io/` within a few minutes.

## Custom domain (e.g. pahp.khu.ac.kr)
1. Ask the university IT office to create a CNAME record pointing the subdomain to `<account>.github.io`.
2. In Settings → Pages → Custom domain, enter the subdomain and turn on "Enforce HTTPS".

## Updating
- Add a photo: save a square JPG into `images/` and replace the `<span class="av">..</span>` placeholder next to the person's name with `<img class="av" src="images/<file>.jpg" alt="<Name>">`.
- Add a paper: in `index.html`, find `const P=[` and add an entry `{"t":"Authors. Title. Journal.","y":2026,"s":"pub","c":1}` (`c:1` marks corresponding author).

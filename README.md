# Dr. Shama Eye Clinic: website (GitHub Pages build)

Static build of the bilingual (Arabic / English) website for Prof. Dr. Ahmed
Shama's eye clinic in Smouha, Alexandria.

Live address: <https://megamind2999.github.io/dr-shama-clinic/>

## Publish

1. Create a public repository named **dr-shama-clinic** on the MegaMind2999
   GitHub account (leave it empty: no README, licence or .gitignore).
2. From this folder:

   ```sh
   git remote add origin https://github.com/MegaMind2999/dr-shama-clinic.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a
   branch**, then pick **main** and **/ (root)** and save. The site is live at the
   address above a minute or two later.

## Notes

- These files are generated. Don't edit them here: change the source project and
  rebuild. Every page and link expects the `/dr-shama-clinic/` sub-folder, so a
  repository with a different name needs a rebuild.
- `.nojekyll` must stay: without it GitHub Pages hides the `_next` folder and
  the site loses its styles and scripts.
- The root `index.html` sends visitors to `ar/` or `en/` (their saved choice,
  then their browser language, then Arabic).
- GitHub Pages has no server, so the call-back request form is not included;
  visitors are asked to call instead.

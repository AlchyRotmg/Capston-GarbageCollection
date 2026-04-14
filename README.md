# Corner Brook Garbage Collection App

This project is set up to deploy on **GitHub Pages without gh-pages**.

## Publish on GitHub Pages

1. In the project folder run:
   ```bash
   npm install
   npm run build
   ```
2. Commit and push the generated `docs` folder to GitHub.
3. In GitHub go to **Settings → Pages**.
4. Set the source to **Deploy from a branch**.
5. Choose:
   - **Branch:** `main`
   - **Folder:** `/docs`
6. Save.

The app uses relative asset paths, so it does not need a hardcoded repository name in `vite.config.js`.

## Development

```bash
npm install
npm run dev
```

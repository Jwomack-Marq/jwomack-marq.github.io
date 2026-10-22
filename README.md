# jwomack-marq.github.io

The root of the GitHub Pages domain. It exists for two reasons:

- **`.well-known/assetlinks.json`** proves the Contraseña Flashcards Android app
  (package `io.github.jwomack_marq.contrasena`, built from
  [contrasena-anki](https://github.com/Jwomack-Marq/contrasena-anki)) belongs to
  this site, so it opens full-screen instead of showing a browser address bar.
  Android only looks for the file at the domain root, never under a project path.
  The fingerprint is the SHA-256 of the app's signing certificate.
- **`index.html`** redirects to the app, so `jwomack-marq.github.io` alone works.

`.nojekyll` stops the Pages build from dropping the `.well-known` folder
(Jekyll skips dot-folders).

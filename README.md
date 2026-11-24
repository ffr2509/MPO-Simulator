# MPO Simulator

A classroom pump panel simulator for training motor pump operators (MPOs), modeled on the pump panel of Asbury Park Fire Department Engine 1 (2000 GPM pump, 500 gallon tank) with an FRC PumpBoss-style pressure governor.

It runs entirely in the browser: no internet is needed once it has been opened, and it can be installed on an iPad's home screen like an app.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole simulator (panel, hydraulics model, governor, sound, instructor variables) |
| `manifest.webmanifest` | App name, icon and full-screen settings for the home screen |
| `sw.js` | Offline support: keeps a saved copy so it runs with no connection |
| `icons/` | Home-screen icons |

## Install on an iPad

1. In this repository, go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the **main** branch and the **/(root)** folder, and press **Save**.
2. After a minute or two the page shows the site address, something like `https://<your-username>.github.io/MPO-Simulator/`.
3. Open that address in **Safari** on the iPad, tap the **Share** button, then **Add to Home Screen**.
4. Open it once from the new home-screen icon while connected, so the offline copy is saved. After that it works with no internet.

## Updating

Change `index.html` and commit. The iPad picks up the new version the next time the app is opened with a connection.

## Instructor notes

- Press and hold the department patch for one second to open the hidden instructor variables (kinks, bursts, supply problems, delayed or patch-tap triggers, hide the answer key).
- Settings (on the right side) holds presets, hose friction coefficients, sound volume and engine sound choice.

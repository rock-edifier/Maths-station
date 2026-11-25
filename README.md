# Maths Station

A maths practice app for children aged 5–10, made for the iPad.

- Questions are generated at random in 16 levels, from number bonds to fractions, percentages and word problems.
- The strategies and "Show me a trick" hints are inspired by Greg Tang's number-sense approach: partners of 10, making tens, doubles, adding the big parts first, counting up to subtract and breaking numbers apart.
- There's a whiteboard for working out with an Apple Pencil, and a pop-up number pad for the answer.
- Each level has four speeds (Practice, Beginner, Advanced, Expert), with a timer bar on the timed ones.
- Gold medals and cups for perfect rounds, with players, results and tricky questions saved per child.

Everything is in `index.html`. It needs no server code, build step or internet connection after the first visit.

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | Name, colours and icons when added to the Home Screen |
| `sw.js` | Lets the app work offline after the first visit |
| `icons/` | Home Screen and browser icons |

## Put it on GitHub Pages

1. On GitHub, create a new repository, e.g. `maths-station`.
2. Choose **Add file → Upload files**. Drag in everything from this folder, including the `icons` folder, then **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment** choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. After a minute or two the app is live at `https://<your-username>.github.io/maths-station/`.

## Install it on an iPad

1. Open the link in **Safari**.
2. Tap the **Share** button, then **Add to Home Screen**.
3. It opens full screen like an app and works without wifi.

## Updating

1. Upload the new `index.html` over the old one.
2. In `sw.js`, change the `VERSION` line (e.g. to `maths-station-v2.2`) and upload that too.
3. Open the app on the iPad while online. It picks up the new version the next time it opens.

## Saved progress

Players, results and medals are saved in the browser on each iPad (`localStorage`). They aren't shared between devices.

- Deleting the Home Screen app or clearing Safari's website data erases them.
- Progress made in Safari is kept separately from progress made in the Home Screen app.

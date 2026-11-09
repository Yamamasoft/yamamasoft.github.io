# yamamasoft.github.io

The public website of Yamama Software, served by GitHub Pages at **https://yamamasoft.github.io/**. It holds the privacy policies of our games and apps.

## Pages

| Page | URL |
|---|---|
| Home | https://yamamasoft.github.io/ |
| Tap&Pop | https://yamamasoft.github.io/tappop/ |
| Tap&Pop privacy policy, English | https://yamamasoft.github.io/tappop/privacy/ |
| Tap&Pop privacy policy, Arabic | https://yamamasoft.github.io/tappop/privacy/ar/ |
| Tap&Pop data deletion (for Google Play's Data safety form) | https://yamamasoft.github.io/tappop/privacy/#delete-data |

**These URLs are permanent.** They are entered in Google Play Console and built into the game. Never rename this repository, the `Yamamasoft` organisation or the folders, and keep the repository public: on GitHub's free plan a private repository cannot publish a site.

## Layout

```text
index.html                     Home: the list of apps
404.html                       Page not found
.nojekyll                      Serve the files as they are (no Jekyll build)
assets/site.css                One stylesheet for every page (light and dark, English and Arabic)
assets/fonts/                  Noto Sans Arabic, cut to the characters the pages use, and its licence (SIL OFL 1.1)
tappop/index.html              Tap&Pop's page
tappop/privacy/index.html      Privacy policy, English
tappop/privacy/ar/index.html   Privacy policy, Arabic
tappop/assets/                 Tap&Pop art from the game, sized for the web
```

Plain HTML and CSS: no build step, no JavaScript, no cookies, no trackers. Links between pages are relative; only the canonical, language and link-preview addresses in each page's `<head>` name `https://yamamasoft.github.io/`.

The Tap&Pop art in `tappop/assets/` is © Yamama Software. Noto Sans Arabic is under the SIL Open Font License 1.1 (`assets/fonts/OFL.txt`).

## Updating a policy

1. Change the English and the Arabic page together; they must say the same thing.
2. Update the "Last updated" date at the top of both pages: the visible text and the `datetime` attribute.
3. Commit and push to `main`. GitHub Pages republishes within a few minutes.
4. If the change is important, for example the game starts collecting a new kind of information, tell players in the game or on its store page, as the policy promises.

## Adding another app

1. Copy `tappop/` to a new folder named after the app. The folder name becomes part of its permanent URL.
2. Replace the art in its `assets/` folder and rewrite both policy pages for what that app actually does.
3. Add the app to `index.html`.

## Publishing settings

Repository **Settings → Pages → Build and deployment**: Source **Deploy from a branch**, branch **`main`**, folder **`/ (root)`**.

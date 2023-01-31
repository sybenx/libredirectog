# LibRedirect OG

### Forked from Libredirect at version 2.3.4 before the removal of features: latency test, wikiless, instance toggle in pop-up, etc.

A web extension that redirects YouTube, Twitter, Instagram... requests to alternative privacy friendly frontends and backends.

[![Matrix Badge](https://img.shields.io/matrix/libredirect:matrix.org?label=matrix%20chat)](https://matrix.to/#/#libredirect:matrix.org)
[![Firefox users Badge](https://img.shields.io/amo/users/libredirect?label=Firefox%20users)](https://addons.mozilla.org/firefox/addon/libredirect/)

<img src ="./img/1.png" width=350>&nbsp;
<img src ="./img/2.png" width=350>&nbsp;
<img src ="./img/3.png" width=350>&nbsp;
<img src ="./img/4.png" width=350>&nbsp;

- Youtube => [Invidious](https://github.com/iv-org/invidious), [Piped](https://github.com/TeamPiped/Piped), [Piped-Material](https://github.com/mmjee/Piped-Material), [CloudTube](https://sr.ht/~cadence/tube/), [FreeTube](https://github.com/FreeTubeApp/FreeTube), [Yattee](https://github.com/yattee/yattee)
- Youtube Music => [Beatbump](https://github.com/snuffyDev/Beatbump), [Hyperpipe](https://codeberg.org/Hyperpipe/Hyperpipe)
- Twitter => [Nitter](https://github.com/zedeus/nitter)
- Instagram => [Bibliogram](https://sr.ht/~cadence/bibliogram/)
- TikTok => [ProxiTok](https://github.com/pablouser1/ProxiTok)
- Reddit => [Libreddit](https://github.com/spikecodes/libreddit#instances), [Teddit](https://codeberg.org/teddit/teddit#instances)
- Imgur => [Rimgo](https://codeberg.org/video-prize-ranch/rimgo)
- Wikipedia => [Wikiless](https://codeberg.org/orenom/wikiless)
- Medium => [Scribe](https://sr.ht/~edwardloveall/scribe/)
- Quora => [Quetre](https://github.com/zyachel/quetre)
- IMDb => [libremdb](https://github.com/zyachel/libremdb)
- PeerTube => [SimpleerTube](https://git.sr.ht/~metalune/simpleweb_peertube)
- LBRY/Odysee => [Librarian](https://codeberg.org/librarian/librarian), [LBRY Desktop](https://lbry.com/get)
- Search => [SearXNG](https://github.com/searxng/searxng), [SearX](https://searx.github.io/searx/), [Whoogle](https://benbusby.com/projects/whoogle-search/), [LibreX](https://github.com/hnhx/librex/)
- Translate => [SimplyTranslate](https://git.sr.ht/~metalune/simplytranslate_web), [LingvaTranslate](https://github.com/TheDavidDelta/lingva-translate), [LibreTranslate](https://github.com/LibreTranslate/LibreTranslate)
- Maps => [OpenStreetMap](https://www.openstreetmap.org/), [FacilMap](https://github.com/FacilMap/facilmap)
- Send Files => [Send](https://gitlab.com/timvisee/send)

**Note**: The Extension will be using random instances by default. You can modify this and add custom instances too.

## Development

### Install Dependencies

[Node.js](https://nodejs.org/) latest LTS is recommended

```
npm update
npm install
```

If you are modifying `config.json` or any files ending with .ejs, you need to run the following command to render html:

```
npm run ejs
```

### Build the extention zip archive:

```
npm run build
```

### Run automated tests

```
npm run test
```

### Test in Firefox

```
npm run start
```

### Install temporarily

1. open `about:addons`
2. type in the address bar `about:debugging`
3. press `load temporarily addon`

### Install in Firefox ESR, Developer Edition, Nightly

1. open `about:config`
2. set `xpinstall.signatures.required` to `false`
3. open `about:addons`
4. click on the gear shaped `settings` button and select `Install Add-on From File...`
5. select `libredirect-VERSION.zip` from `web-ext-artifacts` folder

### Install in Chromium browsers

1. open `chrome://extensions`
2. enable `dev mode`
3. select `load unpacked extension`
4. select `src` folder

Forked from [Libredirect](https://github.com/SimonBrazell/privacy-redirect)

Forked from [Privacy Redirect](https://github.com/SimonBrazell/privacy-redirect)

# Momo Dev Story — web player

https://2026.momothezencat.workers.dev/

Plays `public/momo_dev_story.nds` in the browser with [EmulatorJS](https://emulatorjs.org)
(loaded from its CDN). On phones EmulatorJS shows an on-screen gamepad; the
bottom DS screen is touchable.

The **↑↑↓↓←→←→BA** button (or the <kbd>`</kbd> key) types the secret code,
which jumps one step ahead in the game (next stage).

## Update the ROM

```sh
cd ..   # the game repo
make
cp momo_dev_story.nds 2026/public/
```

## Deploy

```sh
npx wrangler deploy
```

Local preview: `npx wrangler dev`.

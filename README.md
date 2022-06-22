# vitejs-vite-ccuzee

[Edit on StackBlitz ⚡️](https://stackblitz.com/edit/vitejs-vite-ccuzee)


This reproduces an issue with https://github.com/preactjs/preset-vite and vite 3.

Steps:
1. `npm i --legacy-peer-deps` (required because preset-vite does not allow vite 3 in its peerDependencies).
2. `npm run build`
3. `npm run preview`
4. Open the browser, see a blank screen, check the console and notice `Uncaught ReferenceError: require is not defined`

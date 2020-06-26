# React Native BBS Signatures (w/ asm.js fallback)

This repo houses a sample React Native app which uses `bbs-signatures` from [MATTR Global](https://github.com/mattrglobal/bbs-signatures). It is using the `asm.js` fallback as WASM is unsupported in React Native currently.

## Output

![Output](app_screenshot.jpg 'App Screenshot')

## Setup

```
yarn
```

Run the metro bundler with additional memory because the `asm.js` dependency is large and will result in Javascript Out-Of-Memory under the default settings.

Linux/MacOS
`NODE_OPTIONS=--max_old_space_size=8192 yarn start`

Windows
`set NODE_OPTIONS="--max-old-space-size=8192" && yarn start`

This WILL take some time the first time because of the large dependancy size, so go take a break.

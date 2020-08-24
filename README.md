This repository is result of running following commands on Aug 24, 2020 around 14:00 UTC:

```sh
yarn create react-app . --template typescript # log lines 1-150
npx sb init # log lines 151-519
```

Installation log could be found at [install.log file](./install.log)

Trying to run `yarn build-storybook` results to an error. See [build.log file](./build.log)

All default stories except of `Introduction.stories.mdx` producing stack traces like:

```
WARN ./src/stories/Button.stories.tsx
WARN Module build failed (from ./node_modules/@storybook/source-loader/dist/index.js):
WARN TypeError: Cannot read property 'start' of undefined
WARN     at handleExportedName (/home/guria/ws/sandbox/my-app/node_modules/@storybook/source-loader/dist/abstract-syntax-tree/parse-helpers.js:130:19)
WARN     at Controller.enter (/home/guria/ws/sandbox/my-app/node_modules/@storybook/source-loader/dist/abstract-syntax-tree/traverse-helpers.js:161:58)
```

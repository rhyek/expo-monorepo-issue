# expo-monorepo-issue

## with npm workspaces

- have an npm version that supports workspaces (>=7)
- run `npm i` in the root dir
- in `apps/react-native-app` run `npm run android`
- load app in the expo client
- get error:

```bash
› Metro waiting on exp://192.168.0.11:19001
› Scan the QR code above with Expo Go (Android) or the Camera app (iOS)

› Press a │ open Android
› Press i │ open iOS simulator
› Press w │ open web

› Press r │ reload app
› Press m │ toggle menu
› Press d │ show developer tools
› shift+d │ toggle auto opening developer tools on startup (disabled)

› Press ? │ show all commands

Logs for your project will appear below. Press Ctrl+C to exit.
Error: Cannot resolve entry file: The `main` field defined in your `package.json` points to a non-existent path.
    at getEntryPointWithExtensions (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/@expo+config@6.0.14/node_modules/@expo/config/src/paths/paths.ts:83:17)
    at getEntryPoint (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/@expo+config@6.0.14/node_modules/@expo/config/src/paths/paths.ts:42:10)
    at resolveEntryPoint (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/xdl@59.2.22/node_modules/xdl/src/tools/resolveEntryPoint.ts:21:17)
    at getManifestResponseAsync (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/xdl@59.2.22/node_modules/xdl/src/start/ManifestHandler.ts:246:20)
    at getManifestResponseFromHeadersAsync (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/xdl@59.2.22/node_modules/xdl/src/start/ManifestHandler.ts:190:10)
    at /Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/xdl@59.2.22/node_modules/xdl/src/start/ManifestHandler.ts:151:55
    at call (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/connect@3.7.0/node_modules/connect/index.js:239:7)
    at next (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/connect@3.7.0/node_modules/connect/index.js:183:5)
    at Function.handle (/Users/carlos/.nvm/versions/node/v16.13.1/pnpm-global/5/node_modules/.pnpm/connect@3.7.0/node_modules/connect/index.js:186:3)
    at handle (/Users/carlos/Dev/test/expo-monorepo-issue/node_modules/connect/index.js:91:14)
```

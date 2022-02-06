# expo-monorepo-issue

## with npm workspaces

- have pnpm installed
- run `pnpm i` in the root dir
- in `apps/react-native-app` run `pnpm android`
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
Error: EISDIR: illegal operation on a directory, read
    at Object.readSync (node:fs:723:3)
    at tryReadSync (node:fs:433:20)
    at Object.readFileSync (node:fs:479:19)
    at UnableToResolveError.buildCodeFrameMessage (/Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/node-haste/DependencyGraph/ModuleResolution.js:347:17)
    at new UnableToResolveError (/Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/node-haste/DependencyGraph/ModuleResolution.js:333:35)
    at ModuleResolver.resolveDependency (/Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/node-haste/DependencyGraph/ModuleResolution.js:211:15)
    at DependencyGraph.resolveDependency (/Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/node-haste/DependencyGraph.js:413:43)
    at /Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/lib/transformHelpers.js:317:42
    at /Users/carlos/Dev/test/expo-monorepo-issue/node_modules/.pnpm/metro@0.64.0/node_modules/metro/src/Server.js:1471:14
    at Generator.next (<anonymous>)
```

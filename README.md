# svelte-dependency-issue

- `git clone` this repo
- `cd my-lib`
- `pnpm i`
- `svelte-kit package`
- `cd ../my-app`
- `pnpm i`
- `svelte-kit build`

throws following error

```
Error [ERR_MODULE_NOT_FOUND]: Cannot find package 'dayjs' imported from svelte-dependency-issue/my-app/.svelte-kit/output/server/entries/pages/__layout.svelte.js
 at new NodeError (node:internal/errors:371:5)
    at packageResolve (node:internal/modules/esm/resolve:930:9)
    at moduleResolve (node:internal/modules/esm/resolve:976:18)
    at defaultResolve (node:internal/modules/esm/resolve:1078:11)
    at ESMLoader.resolve (node:internal/modules/esm/loader:530:30)
    at ESMLoader.getModuleJob (node:internal/modules/esm/loader:251:18)
    at ModuleWrap.<anonymous> (node:internal/modules/esm/module_job:79:40)
    at link (node:internal/modules/esm/module_job:78:36)
```

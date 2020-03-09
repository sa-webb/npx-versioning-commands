# [npx](https://www.npmjs.com/package/npx) commands

npx is a tool that can avoid polluting global configuration when running global commands.

## Latest version

To execute the **newest** npm command using npx.
`npx --ignore-existing <package> --version`

Sometimes deep symoblic links can trigger stochastic behavior using npm. This can result from multiple re-installs. If experiencing this behavior, add the `--ignore-existing` flag so that - If this flag is set, npx will not look in $PATH, or in the current package's node_modules/.bin for an existing version before deciding whether to install.

## Versioning

To execute **different versions**.

### Current

`npx node --version` or `npx node -v`

### Specific

e.g. Node10
`npx node@10 --version` or `npx node@10 -v`

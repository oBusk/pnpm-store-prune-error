# pnpm-store-prune-error
Reproduction of pnpm store prune error

See [pnpm/pnpm#10131](https://github.com/pnpm/pnpm/issues/10131)

## Reproduction Steps

1. Add node to pnpm store

   - Either by installing a package that has node as a runtime dependency (like this repo) `pnpm install`
   - Or by adding node directly to the store `pnpm store add node@runtime:22`

2. Run `pnpm store prune`
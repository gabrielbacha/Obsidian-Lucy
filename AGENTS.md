# Repository instructions

## Releases

- Obsidian release tags must exactly match `manifest.json.version`.
- Never prefix release tags with `v`: use `1.0.8`, not `v1.0.8`.
- Use `npm run release` to create patch releases; `.npmrc` removes npm's default `v` prefix.
- Before considering a release complete, verify that a GitHub release exists for the exact manifest version and contains `manifest.json` and `theme.css`.

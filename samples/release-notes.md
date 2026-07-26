# Release Notes

A short document with clear top-level sections. Useful for trying Presentation
Mode (Cmd+Shift+P), where each heading becomes a slide.

# Version 3.2

Shipped 2026-07-20.

- Rewrote the indexer to run incrementally
- Cut cold start from 4.1s to 0.8s
- Fixed a crash when opening files over 50 MB

# Version 3.1

Shipped 2026-06-14.

- Added dark mode support across all views
- New keyboard shortcut for quick search
- Improved handling of files with mixed line endings

# Version 3.0

Shipped 2026-05-02. A major release.

## Breaking changes

The `legacy` export was removed. Migrate to the standard entry point:

```diff
- import thing from "package/legacy";
+ import { thing } from "package";
```

## New

- Plugin system with a documented lifecycle
- Configuration file support
- Offline mode

## Fixed

| Issue | Description |
|---|---|
| #412 | Search returned stale results after a rename |
| #418 | Export dropped trailing whitespace |
| #431 | Window position was not restored on relaunch |

# Roadmap

- [x] Incremental indexing
- [x] Plugin system
- [ ] Collaborative editing
- [ ] Mobile companion app

> Dates are targets, not commitments.

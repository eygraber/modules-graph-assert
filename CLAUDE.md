# CLAUDE.md

This repository is a fork of [eduardbosch/modules-graph-assert](https://github.com/eduardbosch/modules-graph-assert). It publishes to Maven Central under the `com.eygraber` group. The plugin ids are `com.eygraber.module.graph.assertion` and `com.eygraber.module.graph.assertion.settings`.

## Branches

| Branch     | Purpose                                                                |
|:-----------|:-----------------------------------------------------------------------|
| `master`   | Upstream syncs only. It mirrors `eduardbosch/modules-graph-assert`.    |
| `eygraber` | The default branch. Target all changes here.                           |

Do not commit fork changes to `master`. Sync it from upstream only.

## Pull upstream work

1. Sync upstream `master` into `master`.
2. Rebase `eygraber` onto `master`.

## Publish

To release a version, run the `release` workflow on `eygraber` with `workflow_dispatch`. Its required `number` input selects the release in the current series. The series prefix is hardcoded in [release.yml](/.github/workflows/release.yml).

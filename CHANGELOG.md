# Changelog

All notable changes to rules_github. The format is loosely
[Keep a Changelog](https://keepachangelog.com/) — version headers
mirror the published bazel-registry entries.

## 0.1.1 — public bzl_library targets

- Mark `bzl_library` targets as public so downstream stardoc builds in
  consumer repos (rules_bun, rules_postgres, …) can depend on them.

## 0.1.0 — initial release

- First cut of shared Bazel repository rules for fetching content from
  GitHub releases: `github_binary_repository` (per-platform release
  asset URLs) and `github_source_repository` (tag tarball URLs). Acts
  as the common substrate beneath fastverk's other `rules_*` modules.

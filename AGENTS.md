# AGENTS.md

Technical operating rules for this organization defaults repository.

## 1. Repository Scope

- Stores the public organization profile (`profile/README.md`), self-contained animated SVG banners (`profile/assets/banners/`), brand vectors (`profile/assets/trademark/`), `CODEOWNERS`, and default `SECURITY.md`.
- Single permanent protected branch (`main`); submit changes via short-lived branch pull requests.

## 2. Toolchain & Validation

- Write all documentation, asset descriptions, and commit messages in English.
- Keep every SVG banner and brand vector self-contained: no scripts, no embedded text, no external fonts, and no remote requests.
- Do not run automated code formatters; preserve license files byte-for-byte.

## 3. Code Layout & Architecture

- `profile/README.md`: public organization overview and constellation table.
- `profile/assets/banners/*.svg`: standalone animated SVG banners referenced by repositories.
- `profile/assets/trademark/*.svg`: vector logo and background marks.
- `CODEOWNERS` & `SECURITY.md`: review ownership and default vulnerability disclosure policy.

## 4. Commit, Dependency & License Policy

- Set Git Author and Committer identically to the repository maintainer account using a GitHub noreply email.
- Format commits as `type(scope): description` (3 to 6 lowercase words, no period), one blank line, and 3+ consecutive `- **Label**: text` bullets (3 to 10 words each) without trailers.
- Zero external runtime dependencies; documentation and assets are licensed under the Apache License 2.0 (`Copyright (c) 2026 Natuleadan`).

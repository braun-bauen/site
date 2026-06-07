# Braun Bauen Website

The marketing and content site for Braun Bauen, built using Astro, TailwindCSS, and AlpineJS.

## Content

- [Home](https://braunbauen.com): landing page with informative content and portfolio.
- [About](https://braunbauen.com/about): digital resume optimized for printing.
- [Cover Letter](https://braunbauen.com/cover-letter): simple editable text area with pre-determined formatting to easily create on-brand cover letters.

## Runtime and Tooling

- App runtime/build tool: Astro
- Package manager: pnpm
- Lint/format/check tooling: vite-plus
- Node version: `24.16.0` from `.node-version`

## Commands

All commands are run from the project root.

| Command             | Action                                         |
| :------------------ | :--------------------------------------------- |
| `pnpm install`      | Install dependencies                           |
| `pnpm dev`          | Start the Astro dev server at `localhost:4321` |
| `pnpm build`        | Build the production site into `./dist/`       |
| `pnpm preview`      | Preview the production build locally           |
| `pnpm check`        | Run the full vite-plus checks                  |
| `pnpm check:fix`    | Run checks and apply safe fixes                |
| `pnpm lint`         | Run linting only                               |
| `pnpm lint:fix`     | Run linting and apply fixes                    |
| `pnpm format`       | Format files                                   |
| `pnpm format:check` | Verify formatting without writing changes      |
| `pnpm astro ...`    | Run Astro CLI commands directly                |

## Local Setup

Use a Node version manager that reads `.node-version`, then run:

```sh
pnpm install
pnpm dev
```

## CI/CD

Recommended baseline for CI:

```sh
pnpm install --frozen-lockfile
pnpm check
pnpm build
```

If you want formatting to be reported separately in CI, use:

```sh
pnpm install --frozen-lockfile
pnpm format:check
pnpm lint
pnpm build
```

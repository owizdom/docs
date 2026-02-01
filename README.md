# Config Validator Docs

Documentation for [Config Validator](https://github.com/owizdom/config-validator), built with [Mintlify](https://mintlify.com).

## Run locally

1. **From the repo root** (where `docs.json` is):

   ```bash
   cd config-validator-docs
   npx mint dev
   ```

   Or with the Mint CLI installed globally:

   ```bash
   mint dev
   ```

2. Open **http://localhost:3000** in your browser.

3. If you see 404s, try **http://localhost:3000/intro** or **http://localhost:3000/index**. Ensure you're on the latest Mint CLI: `npm i -g mint` then `mint update`.

## Deploy to Mintlify

1. Create a project at [dashboard.mintlify.com](https://dashboard.mintlify.com).
2. Connect this repository.
3. Mintlify builds from the default branch; pushes update the site.

## Structure

- **docs.json** — Mintlify config (theme, navigation, navbar, footer). Structure matches the [Mintlify starter](https://github.com/mintlify/starter).
- **Root** — All `.mdx` pages live next to `docs.json`: `index.mdx`, `intro.mdx`, `quickstart.mdx`, `troubleshooting.mdx`, plus `features/`, `cli/`, `sdk/` subfolders. Navigation paths in `docs.json` are relative to the repo root (e.g. `intro`, `features/validation`).
- **public/** — Static assets (e.g. `favicon.svg`).

## If it still doesn’t work

- **Schema errors:** Your Mintlify CLI may expect a different schema. Run `mint update` or check [Mintlify docs](https://mintlify.com/docs).

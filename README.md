# MigmaAI Docs

This repository contains the MigmaAI documentation site.

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview the documentation changes locally:

```
npm i -g mint
```

Run the dev server at the root (where docs.json is):

```
mint dev
```

API endpoint pages are auto-generated from `api-reference/openapi.json` via the `openapi` field in `docs.json`.

### Publishing Changes

Push to the default branch to deploy. If you use the Mintlify GitHub App, changes will auto-deploy from this repo.

#### Troubleshooting

- If the dev environment isn't running, try `mint install` to re-install dependencies.
- If a page loads as 404, ensure you're in the folder with `docs.json`.

# Uyu Docs

This repository powers the public-facing documentation for the **Uyu** platform. It is built with [Mintlify](https://mintlify.com), rendered from MDX content, and deployed automatically through the Mintlify dashboard.

## Project structure

- `docs.json` – site configuration (navigation, branding, tabs, CTA buttons)
- `index.mdx`, `quickstart.mdx`, etc. – high-level guides published under the **Development** tab
- `api-reference/` – OpenAPI-powered reference pages
- `snippets/` – reusable MDX snippets that can be embedded in multiple guides

## Local development

1. Install the CLI if needed: `npm i -g mint`
2. Start the preview server at the repo root: `mint dev`
3. Visit `http://localhost:3000` for live reload previews

Common helpers:

- `mint broken-links` – scan for invalid internal/external links
- `mint dev --port 4000` – run the preview server on a custom port

## Deploying changes

1. Install the Mintlify GitHub app from the [dashboard](https://dashboard.mintlify.com/settings/organization/github-app).
2. Push to the default branch. The GitHub app builds and deploys automatically.
3. Monitor status checks on the PR to ensure the release succeeded.

## Support & troubleshooting

- Run `mint update` if the local renderer drifts from production.
- Delete `~/.mintlify` if the CLI cache becomes corrupted.
- Join the [Mintlify community](https://mintlify.com/community) or email `hi@mintlify.com` for help.

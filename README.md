# Firedrill documentation

Developer documentation for [Firedrill](https://firedrill.run), built with Mintlify.

## Preview locally

Install the Mintlify CLI, then start the preview from this directory:

```bash
npm install --global mint
mint dev
```

Open the local URL printed by the CLI. Before pushing a documentation change, run:

```bash
mint validate
mint broken-links --check-anchors --check-redirects --check-snippets
mint a11y
```

## Source of truth

- The open-source framework and local SDK are maintained by the [`firedrill-tools`](https://github.com/firedrill-tools) organization.
- `api-reference/openapi.json` is copied from the current hosted control-plane contract.
- The CLI reference is generated from the current release-candidate CLI.

Documentation must describe executable behavior. A route, type, or roadmap item alone is not proof that a feature is available.

# CLAUDE.md

## Repository Overview

This repository hosts a single static HTML privacy policy document for **PokeAPI Assistant**, a free custom GPT (ChatGPT plugin) that answers Pokemon-related questions by querying the public [PokeAPI](https://pokeapi.co).

## Repository Structure

```
privacy/
└── privacy-policy.html   # The sole file — a self-contained HTML privacy policy page
```

There is no application code, build system, test suite, or dependency manager in this repository.

## File: privacy-policy.html

A standalone, self-contained HTML document. Key characteristics:

- **No external dependencies** — all CSS is inline within a `<style>` block in `<head>`
- **Single-column layout** — max-width 720px, centered, with system font stack
- **Sections covered**: Overview, Data Collection, Third-Party Services, Cookies and Tracking, Children's Privacy, Changes to This Policy, Contact
- **Last updated**: March 12, 2026

### Editing conventions

- Keep all styles in the `<style>` block in `<head>` — do not add external stylesheets or JavaScript
- Update the `Last updated` date in the `<p class="updated">` element whenever the policy content changes
- Maintain semantic HTML structure (`<h1>`, `<h2>`, `<p>`) — no `<div>` soup
- Keep the document concise; this is a legal/compliance document, not a marketing page

## Development Workflow

There is no build, compile, or deploy step. To make changes:

1. Edit `privacy-policy.html` directly
2. Open the file in a browser to verify rendering
3. Commit with a clear message describing what policy language changed and why
4. Push to the appropriate branch

## Git Conventions

- **Default branch**: `main`
- **Commit messages**: Plain English descriptions of what policy language was added, changed, or removed (e.g., `Update third-party services section to reflect new API usage`)
- No special commit format is enforced

## What This Repository Is Not

- There is no server, backend, or database
- There is no JavaScript framework or bundler
- There are no tests, linters, or CI/CD pipelines
- There is no `.env` file or secrets management

## External References

- **PokeAPI**: https://pokeapi.co/docs/v2
- **OpenAI Privacy Policy**: https://openai.com/policies/privacy-policy

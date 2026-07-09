# Dork File

A single-page tool for building Google dork queries (advanced search operator syntax) without having to memorize them. Built for auditing your own domain's public exposure and authorized OSINT work.

**[Live demo](#)** — replace this with your GitHub Pages link once enabled (see below).

## Features

- **Preset categories** — recon basics, exposed documents, login portals, devices & panels, databases & backups — each with ready-made query templates and plain-English explanations
- **Custom builder** — stack your own `site:`, `filetype:`, `intitle:`, `inurl:`, `intext:`, and exclusion/phrase operators
- **Always-visible operator reference** so you don't have to look up syntax elsewhere
- **One-click copy or open in Google**
- **Saved queries** — persisted locally in your browser via `localStorage`, nothing leaves your machine

## Usage

Open `dork-file.html` in any browser — no build step, no dependencies, no server required.

### Hosting on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Build and deployment," set **Source** to `Deploy from a branch`, pick your default branch and `/ (root)`
4. Your app will be live at `https://<username>.github.io/<repo-name>/dork-file.html`

## Responsible use

This tool only assembles standard Google search queries — it doesn't scan, scrape, or contact any target directly. Use it to review your own organization's public footprint or for work you're authorized to do. Don't use it to locate systems or data you don't have permission to access.

## License

MIT — see [LICENSE](LICENSE).

---

Developed by: George Heath

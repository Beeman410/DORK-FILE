# Dork File

A single-page OSINT toolkit for building Google dork queries and running common recon lookups — no server, no build step, no API keys required for any of the built-in tools.

**[Live demo](#)** — replace this with your GitHub Pages link once enabled (see below).

## Tools included

- **Google Dorks** — preset categories (recon, exposed documents, login portals, devices, databases) plus a custom operator builder, with an always-visible operator reference and locally-saved queries
- **IOC Pivot** — paste an IP, domain, hash, or URL; auto-detects the type and links straight to VirusTotal, AbuseIPDB, Shodan, Censys, crt.sh, or urlscan.io as appropriate
- **DNS Lookup** — live DNS-over-HTTPS queries via Cloudflare's public resolver (A, AAAA, MX, TXT, NS, CNAME, SOA)
- **Username Footprint** — builds direct profile links for a username across ~16 common platforms
- **Reverse Image Search** — paste a hosted image URL, get links into Google Lens, TinEye, Yandex, and Bing Visual Search
- **Archive Lookup** — jump to a URL's Wayback Machine and archive.today history
- **Email Permutation Generator** — generates likely email address patterns from a name and domain
- **EXIF Viewer & Stripper** — reads embedded photo metadata (device, timestamp, GPS) client-side, and produces a metadata-stripped copy for download. Nothing is uploaded anywhere.
- **Threat Intel Links** — reference cards for services that need their own account/API key (Shodan, Censys, VirusTotal, AbuseIPDB, Have I Been Pwned, crt.sh), each with a plain-English description of what it does and a note on what's free to use as-is

## Usage

Open `dork-file.html` in any browser. The EXIF tool and DNS lookup work fully offline-capable/client-side except for the DNS-over-HTTPS request itself.

### Hosting on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Build and deployment," set **Source** to `Deploy from a branch`, pick your default branch and `/ (root)`
4. Your app will be live at `https://<username>.github.io/<repo-name>/dork-file.html`

## A note on API keys

None of the built-in tools require a key. Shodan, Censys, and Have I Been Pwned all require a *secret* API key for programmatic access — and since this is a static site with source visible to anyone (including on GitHub), it can't safely hold a secret key without exposing it. The Threat Intel Links tab points you to those services directly instead of embedding calls to them.

## Responsible use

This tool only assembles search queries and deep links — it doesn't scan, scrape, or contact any target directly beyond what a normal browser visit would do. Use it to review your own organization's public footprint or for work you're authorized to do. Don't use it to locate systems or data you don't have permission to access.

## License

MIT — see [LICENSE](LICENSE).

---

Developed by: George Heath


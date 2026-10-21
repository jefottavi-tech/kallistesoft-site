# kallistesoft.ca

Static site for Kallistesoft, hosted on the GoDaddy web hosting at https://kallistesoft.ca. Every push to `main` uploads it over FTPS (`.github/workflows/deploy-godaddy.yml`, which calls the shared `deploy-ftp.yml` that every site repo uses).

- French at `/`, English at `/en/`. Every page exists in both languages: `block-daily/` ↔ `en/block-daily/`, `void-raid/` ↔ `en/void-raid/` (likewise `neon-pop/`, `neon-snake/`, `neon-stack/`), `confidentialite/` ↔ `en/privacy/`.
- Plain HTML and one stylesheet (`assets/style.css`), with no build step. Push to `main` to publish.
- Preview locally: `python3 -m http.server` and open http://localhost:8000.

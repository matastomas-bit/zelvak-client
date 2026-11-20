# Zelvak Client – web

Statická stránka klienta **Zelvak Client** (Fabric 1.21.11).

## Co tu je

| Soubor | Popis |
| --- | --- |
| `index.html` | Celá stránka včetně odemykacího hesla (bez externích knihoven) |
| `serve.cjs` | Volitelný lokální server (jen `node`, žádné závislosti) |

## Spuštění

Otevři `index.html` v prohlížeči, nebo spusť:

```bash
node serve.cjs
```

a jdi na <http://localhost:8080>.

## Heslo

Přístupové heslo je **1212**. V souboru není uložené jako plaintext – porovnává se
SHA-256 hash, takže se v kódu nedá přečíst.

## Důležité

Heslo je **klientské** – běží v prohlížeči. Odradí náhodné návštěvníky, ale
neumí ochránit obsah před někým, kdo si zobrazí zdrojový kód stránky. Pro
skutečnou ochranu je potřeba řešit přihlášení na serveru (hosting, `.htpasswd`,
Cloudflare Access apod.).

V souborech nejsou žádné přihlašovací údaje, e-maily, tokeny ani osobní data.

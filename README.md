# robertoluttino-it

La pagina personale di Roberto Luttino, robertoluttino.it: lavoro, passioni e
collegamenti agli altri siti.

## Lavorare in locale

```bash
python3 -m http.server 8180 -d docs   # http://localhost:8180/
```

Una pagina sola, scritta a mano, senza build. Identità propria: non usa il
marchio MindContact, lo cita e lo linka.

## Pubblicazione

GitHub Pages dal ramo `main`, cartella `docs/`: ogni push su `main` va online
da solo. Il dominio è in `docs/CNAME` (`robertoluttino.it`); `docs/.nojekyll`
fa servire i file così come sono.

DNS (Cloudflare, solo DNS): `robertoluttino.it` con i record A di GitHub
Pages, `www` in CNAME verso `MindContact.github.io` (GitHub lo reindirizza al
dominio senza `www`).

Nessun indirizzo email nelle pagine.

# 60-Jahre-Rotary-Kitzbuehel (privat)

GitHub-Pages-fähige Struktur für den Ablauf- und Moderationsfragenseite.

## Obfuskation

- Inhalt liegt unter `/bdfb532002f69d/` – ein nicht erratbarer Pfad.
- Root liefert 404, robots.txt sperrt Suchmaschinen.
- **Kein** Passwortschutz – Sicherheit durch nicht-rate-baren Pfad (Security by Obscurity).

## Deployment

```bash
# 1. In neues Repo committen (auf GitHub.com vorher leeres Repo erstellen, z. B. "60-jahre-rotary-kitzbuehel")
cd "60 Jahre Rotary/github_publish"
git init
git add .
git commit -m "Initial publish"
git branch -M main
git remote add origin git@github.com:DEIN_USER/60-jahre-rotary-kitzbuehel.git
git push -u origin main

# 2. GitHub Pages aktivieren:
#    Repo → Settings → Pages → Source: main / (root)

# 3. URL wird sein:
#    https://DEIN_USER.github.io/60-jahre-rotary-kitzbuehel/bdfb532002f69d/
```

## Inhalte aktualisieren

Wenn die HTML-Datei sich ändert:

```bash
cp "../Ablauf_und_Moderationsfragen.html" "bdfb532002f69d/index.html"
git add -A && git commit -m "Update Ablauf" && git push
```

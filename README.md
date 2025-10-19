# Linux Tutorial Hub – Projektkurzinfo

Dieses Repository enthaelt eine massgeschneiderte Hugo-Website fuer den Linux Tutorial Hub. Die Startseite ist so aufgebaut, dass neue Inhalte automatisch in mehreren Bereichen erscheinen.

## Content-Workflows

1. **Neue Guides anlegen**  
   Lege Markdown-Dateien unter `content/posts/<slug>.md` an. Nutze das vordefinierte Frontmatter (`hugo new posts/mein-guide.md`), damit `title`, `date`, `summary`, `level`, `categories`, `tags` und `next_steps` gesetzt werden.
2. **Kategorien & Tags pflegen**  
   Fuege beliebige Werte zu `categories` und `tags` hinzu. Sie werden automatisch in der Themen-Uebersicht sowie in der Tag-Liste auf der Startseite angezeigt.
3. **Hero- und Feature-Texte steuern**  
   Passe statische Landing-Page-Inhalte zentral in `hugo.toml` unter `[params]` an.
4. **Listen- & Detailseiten**  
   Die Vorlagen unter `layouts/_default` aktualisieren automatisch Teaser, Datum, Lesedauer und Next Steps.

## Lokale Vorschau

Installiere Hugo Extended (https://gohugo.io/installation/) und starte die Entwicklungsumgebung mit:

```powershell
hugo server --buildDrafts --disableFastRender
```

## Deployment

Das Projekt generiert statische Assets via `hugo --minify`. Der Output landet standardmaessig im Ordner `public/` und kann auf jeden beliebigen Webserver oder CDN deployt werden.


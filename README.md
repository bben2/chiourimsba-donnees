# Chiourim BA — données

Textes déjà publiés sur [Guemara](https://guemara.vercel.app), [Hassidout](https://hassidout.vercel.app)
et [Halakha](https://halakha.vercel.app), pour le lecteur de l'application iPhone. Dossier lu sur
`https://raw.githubusercontent.com/bben2/chiourimsba-donnees/main/`.

## Contenu

- `catalogue.json` — trois collections : Guemara, Hassidout et moussar, Halakha.
- `guemara/<Traité>/<amud>.json` — feuillet bilingue : texte, Rachi, Tossefot, Roch, Ben Yehoyada, explication, schémas.
- `hassidout/<livre>/<section>.json` — section bilingue (hébreu et français).
- `halakha/<ouvrage>/<section>.json` — section bilingue, avec le résumé « En bref ».

Seules les pages déjà en ligne sont exportées. Pas de Kabbale. Sommaires et guides sans paire hébreu / français exclus.

## Format

JSON UTF-8, compact, clés en français. `catalogue.json` donne pour chaque œuvre le chemin et les unités
dans l'ordre de lecture (`2a`, `2b`… ou `001`, `002`…). Une clé absente signifie que le champ est vide.
`mise_a_jour` est la seule date du dépôt.

## Licences

Traductions françaises, explications, schémas et chiourim : Chiourim BA — Benjamin Abbou,
licence **CC BY 4.0** (`LICENSE`, résumé dans `LICENCE.md`).

Textes hébreux et araméens repris de [Sefaria](https://www.sefaria.org), chacun sous la licence de sa version.
Le Talmud vocalisé William Davidson est sous **CC BY-NC**.

## Mise à jour

Régénéré par `tools/export_donnees.py` dans le dépôt de travail. Relancer le script réécrit ce dossier ;
si les sources publiées n'ont pas changé, les fichiers restent identiques.

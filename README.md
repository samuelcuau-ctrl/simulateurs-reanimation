# Simulateurs de réanimation — le site

Site statique : chaque page est un fichier HTML autonome, sans serveur ni base de données.

## Contenu du dossier

| Adresse sur le site | Fichier |
| --- | --- |
| / (page d'accueil) | `index.html` |
| /ventilation/ | `ventilation/index.html` |
| /fibroscopie/ | `fibroscopie/index.html` |
| /choc-cardiogenique/ | `choc-cardiogenique/index.html` |
| /epuration-extrarenale/ | `epuration-extrarenale/index.html` |
| /ecmo/ | `ecmo/index.html` |
| /mentions-legales/ | `mentions-legales/index.html` (à compléter) |

Plus `manifest.webmanifest` et `icon.svg`, qui permettent d'ajouter le site à l'écran d'accueil d'un téléphone comme une application.

Les liens sont relatifs : l'adresse d'une page ne change jamais quand on met à jour un simulateur. Pour mettre à jour un simulateur, on remplace seulement son fichier.

## Mettre en ligne

N'importe quel hébergeur de site statique convient. Le plus simple est de glisser le dossier entier sur la page de dépôt de l'hébergeur. Pour un suivi des versions, on peut passer par un dépôt GitHub relié à l'hébergeur : chaque modification publiée met le site à jour automatiquement.

Ensuite, on peut relier un nom de domaine (par exemple simulateurs-rea.fr) acheté chez un registrar.

## Avant d'ouvrir au public

- Compléter les mentions légales (éditeur, contact, hébergeur).
- Faire relire les contenus par un pair (protocoles, valeurs de référence).
- Vérifier l'affichage sur téléphone.

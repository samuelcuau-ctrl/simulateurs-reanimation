# Simulateurs de réanimation

Site statique (HTML autonomes, sans build). Une page par simulateur, dans son dossier : `ventilation/`, `fibroscopie/`, `choc-cardiogenique/`, `epuration-extrarenale/`, `ecmo/`, `erreurs/` (chambre à erreurs), `eeg/` (EEG continu). Page d'accueil : `index.html` (tableau `BEDS` : un lit par simulateur, lien relatif vers son dossier).

Partie Formation : `formation/` (page des modules par niveau : socle, approfondissement, consolidation) et un dossier par module-niveau (`formation/ventilation-socle/`). Progression dans le navigateur (`localStorage`, clé `simicu-formation`), sans serveur. Chaque chapitre : cours, exercice au respirateur intégré, quiz (7 questions, 70 %) ; examen (20 questions + 2 épreuves, 80 %, 2 tentatives puis 24 h). Nouveau module : nouveau dossier et nouvelle cellule `url` dans `MODS` de `formation/index.html`.

Règles :
- Quand un simulateur est modifié, remplacer son `index.html` et vérifier dans la même modification que la fiche correspondante de `index.html` (accueil) est à jour (lien, description, étiquettes).
- Nouveau simulateur : nouveau dossier, nouvelle entrée dans `BEDS` avec `st:"on"` et `url:"dossier/"`, et le bandeau « ← Simulateurs de réanimation » en haut de page comme les autres.
- Liens toujours relatifs, pour que le site fonctionne quel que soit l'hébergement.
- Les simulateurs restent indépendants : la formation les complète sans les remplacer.
- QCM : la bonne réponse ne se repère pas à sa longueur ; ordre aléatoire ; explication après le choix.
- Public visé : internes de DES de médecine intensive-réanimation. Textes en français.

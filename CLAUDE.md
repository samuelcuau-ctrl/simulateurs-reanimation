# Simulateurs de réanimation

Site statique (HTML autonomes, sans build). Une page par simulateur, dans son dossier : `ventilation/`, `fibroscopie/`, `choc-cardiogenique/`, `epuration-extrarenale/`, `ecmo/`, `erreurs/` (chambre à erreurs), `eeg/` (EEG continu). Page d'accueil : `index.html` (tableau `BEDS` : un lit par simulateur, lien relatif vers son dossier).

Règles :
- Quand un simulateur est modifié, remplacer son `index.html` et vérifier dans la même modification que la fiche correspondante de `index.html` (accueil) est à jour (lien, description, étiquettes).
- Nouveau simulateur : nouveau dossier, nouvelle entrée dans `BEDS` avec `st:"on"` et `url:"dossier/"`, et le bandeau « ← Simulateurs de réanimation » en haut de page comme les autres.
- Liens toujours relatifs, pour que le site fonctionne quel que soit l'hébergement.
- Public visé : internes de DES de médecine intensive-réanimation. Textes en français.

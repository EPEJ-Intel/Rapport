# Registre d'église — Rapports mensuels

Site statique (HTML/CSS/JS) pour saisir les collectes hebdomadaires
(mercredi, vendredi, dimanche) et générer les deux rapports mensuels
au format EPEJ. Les données sont stockées dans un Google Sheet via
un petit backend Google Apps Script.

## Installation (une seule fois)

1. Créez un Google Sheet vide.
2. Extensions > Apps Script, collez le contenu de `Code.gs.txt`
   (fourni séparément), puis Déployer > Nouveau déploiement
   > Application Web (exécuter en tant que "Moi", accès "Tout le monde").
3. Copiez l'URL de déploiement (se termine par `/exec`).
4. Ouvrez `index.html`, remplacez `PASTE_YOUR_APPS_SCRIPT_URL_HERE`
   par cette URL (variable `APPS_SCRIPT_URL` en haut du `<script>`).
5. Poussez ce dossier sur GitHub, puis activez GitHub Pages
   (Settings > Pages > Branch: main > /root).
6. Votre site est en ligne à l'URL fournie par GitHub Pages.

## Mise à jour

Toute modification de `index.html` doit être repoussée (`git push`)
pour être visible sur le site publié.

# EPEJ — Registre d'église (application installable)

Même application qu'avant (Google Sheet + Apps Script), maintenant **installable** sur
téléphone et ordinateur, utilisable **dans tous les sens** (portrait / paysage) et
**sans perte de données**, même sans internet.

## Mise en ligne (remplace l'ancien contenu du dépôt GitHub)
Copiez tout ce dossier à la racine du dépôt : `index.html`, `manifest.webmanifest`,
`sw.js`, dossier `icons/` (et `Code.gs.txt` inchangé). Puis `git push`.
L'adresse GitHub Pages est en HTTPS : indispensable pour l'installation.

## Installer
- **Android / Chrome** : bouton « ⬇ Installer l'appli » en haut (ou menu ⋮ > Installer l'application).
- **Ordinateur (Chrome / Edge)** : icône d'installation dans la barre d'adresse.
- **iPhone / iPad (Safari)** : Partager > « Sur l'écran d'accueil ».

## Comment les données sont protégées
1. Chaque enregistrement est écrit **d'abord sur l'appareil**, puis envoyé au Google Sheet.
2. Sans réseau : le message indique « Enregistré sur l'appareil » et l'envoi repart
   automatiquement au retour de la connexion (badge en haut : Synchronisé / En attente / Hors ligne).
3. Les 13 derniers mois sont gardés sur l'appareil pour être consultables hors ligne.
4. La déconnexion n'efface rien. Le stockage est demandé en mode « persistant ».
5. Paramètres > Sauvegarde : export / restauration d'un fichier de secours.

Limites : la connexion (première fois) et la création de compte demandent internet ;
l'espace Administration reste en ligne uniquement.
Si vous modifiez l'appli plus tard, changez `VERSION` dans `sw.js` pour forcer la mise à jour.

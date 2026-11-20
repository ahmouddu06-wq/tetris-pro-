# Tetris Pro : APK avec GitHub

GitHub fabrique l'APK pour toi (gratuit), rien à installer.

1. Crée un compte sur github.com, puis un nouveau dépôt (bouton « New »), par exemple `tetris-pro`.
   Public, c'est plus simple pour télécharger l'APK sur ton téléphone.
2. Envoie tout le contenu de ce dossier à la racine du dépôt :
   - « Add file » > « Upload files », glisse les fichiers, puis « Commit changes ».
   - Attention : le dossier caché `.github` est parfois ignoré par le glisser-déposer.
     S'il manque, fais « Add file » > « Create new file », tape le nom
     `.github/workflows/build-apk.yml` et colle le contenu du fichier du même nom.
3. Ouvre l'onglet « Actions » : « Build APK » se lance tout seul (environ 5 minutes).
   Sinon : « Build APK » > « Run workflow ».
4. Quand c'est vert, va dans « Releases » (colonne de droite de la page du dépôt) :
   télécharge `app-debug.apk` depuis ton téléphone et installe-le
   (autorise « sources inconnues » quand Android le demande).

Pour mettre à jour le jeu plus tard : remplace `www/index.html` sur GitHub, une nouvelle release sort.

## Commandes tactiles du jeu
- Glisse gauche / droite : déplacer la pièce
- Touche à gauche / à droite de l'écran : tourner (anti-horaire / horaire)
- Glisse vers le bas : descente douce, flick rapide vers le bas : chute
- Flick vers le haut : réserve
- Deux doigts ou appui long : pause (musique, grille seule, menu)

L'application est verrouillée en mode portrait.

RobotCW
Entraîneur de manipulation et de lecture en morse (CW) pour radioamateurs,
piloté par un keyer K3NG connecté en port série.
Description
RobotCW est un programme Windows qui dialogue avec un keyer K3NG pour
proposer des exercices de morse :
Manipulation : le programme envoie un groupe (chiffres, lettres,
indicatifs, faux indicatifs, mots français) que l'utilisateur doit copier
au clavier et renvoyer via le keyer.
Lecture : le keyer transmet en CW un flux généré par le programme
(chiffres, lettres, indicatifs, mots, citations) que l'utilisateur doit
copier au son.
Une note est calculée en fin de série selon le nombre d'erreurs.
Prérequis
Windows
Un keyer K3NG connecté en port série (USB-série ou port COM classique)
Le port COM du keyer doit être configuré dans `config.cfg`
Installation
Télécharge tous les fichiers de ce dépôt dans un même dossier :
`RobotCW.exe`, `calls.txt`, `citations.txt`, `config.cfg`, `mots.txt`,
`prefix.txt`
Ouvre `config.cfg` avec un éditeur de texte (Bloc-notes) et règle le port
COM de ton keyer :
```
   \[default]
   portcom = com4
   mycall = F4GOP
   maxgroup = 10
   ```
Lance `RobotCW.exe`
Utilisation
Choisis un type d'exercice (Manipulation ou Lecture) via le menu ou les
boutons de l'interface.
Règle la vitesse (WPM), l'espacement entre caractères/mots, et le nombre de
groupes selon tes besoins.
Les fichiers `calls.txt`, `mots.txt`, `citations.txt` et `prefix.txt`
contiennent les listes utilisées pour générer les exercices ; tu peux les
éditer (un élément par ligne) pour personnaliser le contenu.
Fichiers du dépôt
Fichier	Rôle
`RobotCW.exe`	Programme principal
`config.cfg`	Configuration (port COM, indicatif, nombre de groupes)
`calls.txt`	Liste d'indicatifs radioamateurs pour les exercices
`mots.txt`	Liste de mots français
`prefix.txt`	Préfixes utilisés pour générer de faux indicatifs
`citations.txt`	Citations utilisées en exercice de lecture
Auteur
F4GOP

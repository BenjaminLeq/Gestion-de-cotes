# Gestion de côtes

**Gestion de côtes** est une application Windows développée en AutoIt qui permet d’imprimer automatiquement une cote sur une série de feuilles déjà placées dans un copieur ou une imprimante.

La cote est positionnée en haut à droite de chaque page. Sa lettre principale, sa sous-cote et sa mise en forme peuvent être personnalisées avant l’impression.

## Fonctionnalités

- sélection de l’imprimante ou du copieur parmi les périphériques installés ;
- utilisation automatique de l’imprimante Windows par défaut au démarrage ;
- cote principale facultative de **A à Z** ;
- sous-cote facultative de **a à z** ;
- numérotation de **1 à 9999** ;
- ajout automatique des zéros selon le nombre de pages : `A01`, `A001` ou `A0001` ;
- réglage de la distance depuis le haut et la droite de la feuille, en millimètres ;
- choix de la taille de la police et activation facultative du gras ;
- accès aux paramètres du pilote d’impression : bac, format du papier, recto-verso, etc. ;
- fonctionnement sans droits administrateur et sans script PowerShell.

## Exemples de cotation

| Côte | Sous-cote | Page de fin | Résultat |
|---|---|---:|---|
| A | aucune | 99 | `A01` à `A99` |
| D | aucune | 999 | `D001` à `D999` |
| C | a | 9999 | `Ca0001` à `Ca9999` |
| aucune | aucune | 999 | `001` à `999` |

## Utilisation

1. Placez les feuilles à coter dans le bac choisi du copieur ou de l’imprimante.
2. Sélectionnez une cote et, si nécessaire, une sous-cote.
3. Indiquez les pages de début et de fin.
4. Réglez la position et la taille du texte.
5. Sélectionnez l’imprimante ou le copieur.
6. Ouvrez les paramètres d’impression pour choisir le bac, le papier ou le recto-verso.
7. Cliquez sur l’icône d’impression et confirmez l’opération.

> Il est conseillé d’effectuer un essai sur quelques feuilles avant une impression importante afin de vérifier le sens du papier et la position de la cote.

## Prérequis

- Windows ;
- Microsoft Word installé, utilisé par l’application pour préparer et envoyer les pages à l’imprimante ;
- une imprimante ou un copieur installé dans Windows ;
- aucun droit administrateur requis pour utiliser l’application.

## Compilation

1. Installez [AutoIt](https://www.autoitscript.com/site/autoit/).
2. Placez les fichiers suivants dans le même dossier :
   - `GestionDeCotes.au3`
   - `icone.ico`
   - `aide.ico`
   - `imprimer.ico`
   - `parametres.ico`
3. Ouvrez le fichier `.au3` avec **Compile Script to .exe (x64)**.
4. Choisissez `icone.ico` comme icône de l’exécutable, puis lancez la compilation.

Les icônes de l’interface sont intégrées dans l’exécutable pendant la compilation. Elles n’ont donc pas besoin d’être distribuées avec le fichier `.exe`.

## Version

**Version 1.1**

## Auteur

**Benjamin Lequeux**


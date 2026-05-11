# 58376_Texture_HD

Depot de documentation pour une collection locale de textures HD.

Le dossier local associe des textures rangees par series (`Texture_A` a
`Texture_V`) ainsi qu'une image principale. Les fichiers sources de textures et
les medias lourds ne sont pas versionnes dans Git afin de garder le depot
leger et exploitable.

## Raccordement Git

Ce dossier local est raccorde au depot GitHub :

https://github.com/Delfosse-Pascal/58376_Texture_HD

Lors de la creation de ce README, le depot distant ne contenait pas encore de
branche publiee. Le raccordement consiste donc a initialiser le depot Git local,
ajouter `origin`, creer la branche `main`, puis pousser les fichiers de base.

## Contenu local

La collection locale est organisee en dossiers :

| Dossier | Nombre de fichiers |
| --- | ---: |
| Texture_A | 4 564 |
| Texture_B | 3 747 |
| Texture_C | 3 224 |
| Texture_D | 3 952 |
| Texture_E | 2 631 |
| Texture_F | 4 672 |
| Texture_G | 6 730 |
| Texture_H | 3 291 |
| Texture_I | 3 004 |
| Texture_J | 1 857 |
| Texture_K | 1 724 |
| Texture_L | 1 954 |
| Texture_M | 2 462 |
| Texture_N | 2 391 |
| Texture_O | 4 124 |
| Texture_P | 1 423 |
| Texture_Q | 1 832 |
| Texture_R | 1 953 |
| Texture_S | 699 |
| Texture_T | 1 437 |
| Texture_U | 1 365 |
| Texture_V | 703 |

Total local observe : 59 740 fichiers.

## Fichiers exclus du depot

Les elements suivants sont volontairement exclus par `.gitignore` :

- images et textures bitmap (`.jpg`, `.jpeg`, `.png`, `.tif`, `.tiff`, etc.) ;
- documents PDF ;
- videos ;
- archives (`.zip`, `.rar`, `.7z`, `.tar`, etc.) ;
- fichiers audio ;
- fichiers graphiques ou modeles lourds (`.psd`, `.3ds`) ;
- dossiers de textures locaux (`Texture_*/`), afin de ne publier que les
  fichiers de base du depot.

Cette regle permet de conserver la documentation et la configuration Git sans
envoyer les medias ni l'arborescence complete sur GitHub.

## Utilisation

1. Conserver les textures originales dans le dossier local de travail.
2. Mettre a jour ce README lorsque l'organisation, le contenu ou les regles de
   versionnement changent.
3. Ne versionner que les fichiers de documentation, de configuration ou de
   scripts explicitement utiles au suivi du projet.

## Notes de maintenance

- Si des fichiers de texture doivent etre partages, utiliser un stockage adapte
  aux medias lourds plutot que Git classique.
- Si certains fichiers HTML ou scripts contenus dans les dossiers `Texture_*`
  doivent etre suivis plus tard, ajuster `.gitignore` avant de les ajouter.
- Verifier les droits d'utilisation et de redistribution des textures avant
  toute publication publique.

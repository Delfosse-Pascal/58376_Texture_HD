# 58376_Texture_HD

Depot de documentation et portail local pour une collection de textures HD.

Ce depot sert a conserver les fichiers de base du projet : documentation,
configuration Git et page d'accueil locale. Les contenus lourds restent dans
les dossiers de travail locaux et ne sont pas envoyes sur GitHub.

## Objectif du projet

Le projet regroupe une grande collection locale de textures, organisee en
tiroirs de type `Texture_A`, `Texture_B`, etc. Un tiroir `Musique` peut aussi
etre present localement pour accompagner le site avec des fichiers audio.

Le fichier `index.html` place a la racine sert de portail local :

- il centralise les acces aux tiroirs disponibles sur la machine ;
- il donne une vue d'ensemble des pages et ressources locales ;
- il propose une navigation claire pour explorer le contenu ;
- il reste utilisable en local, sans dependance externe obligatoire.

## Depot GitHub

Depot distant raccorde :

https://github.com/Delfosse-Pascal/58376_Texture_HD

La branche principale est `main`.

## Ce qui est versionne

Seuls les fichiers de base doivent etre versionnes :

- `README.md` : documentation du projet ;
- `.gitignore` : regles d'exclusion ;
- `index.html` : accueil local principal, sans integrer les medias eux-memes.

Ces fichiers permettent de comprendre et d'ouvrir le projet localement sans
envoyer les textures, musiques, archives ou autres fichiers lourds.

## Ce qui reste local et n'est pas pousse

Les tiroirs et medias suivants sont volontairement exclus du depot Git :

- dossiers `Texture_*/` ;
- dossier `Musique/` ;
- images et textures bitmap ;
- PDF ;
- videos ;
- archives ;
- fichiers audio ;
- ebooks ;
- fichiers graphiques ou 3D lourds, comme `.psd` et `.3ds`.

Cette separation evite d'alourdir le depot et protege les contenus qui doivent
rester uniquement dans le dossier local de travail.

## Organisation locale observee

Les tiroirs de textures sont organises de `Texture_A` a `Texture_V`. Chaque
tiroir peut contenir :

- des pages HTML historiques ;
- des images de textures ;
- des cartes dans les dossiers `maps` ;
- des miniatures ;
- parfois des archives, modeles 3D ou fichiers sources.

Le tiroir `Musique`, lorsqu'il existe, contient des fichiers audio locaux. Ces
fichiers sont raccordes au portail local mais restent exclus du depot Git.

## Utilisation locale

1. Ouvrir `index.html` a la racine du projet.
2. Naviguer vers les tiroirs de textures ou vers la page musique.
3. Garder les dossiers lourds localement.
4. Ne pousser sur GitHub que les fichiers de documentation et de structure.

## Regles de maintenance

- Ne pas ajouter les dossiers `Texture_*` au suivi Git.
- Ne pas ajouter le dossier `Musique` au suivi Git.
- Ne pas versionner les images, PDF, videos, archives, musiques ou ebooks.
- Mettre a jour ce README quand l'organisation locale change.
- Si un fichier lourd doit etre partage, utiliser un stockage adapte aux medias
  plutot que Git classique.

## Verification avant commit

Avant chaque commit, verifier les fichiers prets a etre envoyes :

```powershell
git status --short --ignored
git diff --cached --name-only
```

Le commit ne doit contenir aucun tiroir local ni fichier media.

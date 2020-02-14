# Projet-Galaxie-2020

## Arborescence

| Fichier | Contenu | Type |
| :-----: | :-----: | :-----: |
| pic_process.py | Toutes les fonctions de traitement d'images | Pack de fonctions |
| minkos.py | Toutes les fonctions relatives aux fonctionelles de M | Pack de fonctions |
| main.py | Calcule les fonctionelles d'une image en format DAT ou FITS | Programme |
| trasismooth.py | Représente les variations des fonctionelles en fonction du lissage des images | Programme |
| morpho.py | Utilise la méthode conventionelle pour calculer les paramètres d'une galaxie | Programme |
| transismoothall.py | Variations des fonctionelles en fonction du lissage séparées en quatre fenêtres | Programme |
| every.py | Compare toutes les fonctionelles de chaque image présente dans un répertoire | Programme |
| test_binary.py | Enregistre les images binaires correspondantes aux maxima/minima locaux | Test |
| test_crop.py | Crop une fonctionelle en l'arretant lorsqu'elle converge vers 0 | Test |

| **Attention: Les fichiers de type "Pack de fonctions" sont utilisés par plusieurs programmes, faire attention lors de leurs modifications.** |
| --- |

## main.py

### Appel:
  `python main.py [FITS ou DAT file] [optional args]`

  - Le chemin vers l'image peut être absolu ou relatif.
  - Les arguments optionels et leurs utilisations peuvent être vus avec `python main.py --h`


### Exemple de résultat:
  ![alt text][Test1]

  [Tous les résultats](osef/all_res.md)


## transismooth.py
  `python transismooth.py [FITS ou DAT file] [optional args]`

  - `-smooth [NOMBRE]` pour le nombre d'itérations. Attention, à plus de 6, le temps de calcul est très long.

### Exemple de résultat:

<img src="datfiles/spiraleBarreeA_Chi.png" alt="drawing" width="300"/><img src="datfiles/spiraleBarreeA_U.png" alt="drawing" width="300"/><img src="datfiles/spiraleBarreeA_F.png" alt="drawing" width="300"/>

## morpho.py
  `python morpho.py [FITS ou DAT file] [optional args]`

## every.py

### Exemple de résultat:

<img src="img/all_chi.png" alt="drawing" width="300"/><img src="img/all_u.png" alt="drawing" width="300"/><img src="datfiles/img/all_f.png" alt="drawing" width="300"/>

## test_binary.py
  `python test_binary.py [FITS ou DAT file] [optional args]` 

### Exemple de résultat:

<img src="img/binary/anim2.gif" alt="drawing" width="300"/>

[Test1]: img/yesyes.png "SuperLesFonctionelles"


## test_binary_interactive.py

  - Possibilité de cliquer sur la courbe pour affichier l'image binarisée correspondante.
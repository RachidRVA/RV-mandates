# Qamar Filmworks — Note de fabrication

Ce dossier est une **référence de design** : deux maquettes HTML (une sombre, une claire) à
reproduire à la main dans **Infomaniak Site Creator**. Rien ici n'est du code à mettre en ligne —
c'est le modèle à partir duquel le site no-code sera reconstruit. Chaque élément a été choisi pour
être **reproductible et modifiable** dans un éditeur glisser-déposer.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `mockup-dark.html` | Maquette complète, palette **sombre** (autonome, s'ouvre hors ligne) |
| `mockup-light.html` | Maquette complète, palette **claire** |
| `wordmarks.html` | Les **trois directions de logotype**, côte à côte |
| `wordmark-w{1,2,3}-dark.png` | Logotypes en PNG transparent, version pour **fond sombre** |
| `wordmark-w{1,2,3}-light.png` | Logotypes en PNG transparent, version pour **fond clair** |
| `assets/portrait-sarah.jpg` | Portrait de Sarah, optimisé pour le web |
| `assets/fonts/fonts-embedded.css` | Les deux polices, intégrées (référence — inutile dans Site Creator) |

## Polices

Deux polices, toutes deux disponibles gratuitement sur **Google Fonts** :

- **Fraunces** — police d'affichage (titres, chiffres, logotype). Serif de caractère, chaleureuse.
  Nom exact Google Fonts : `Fraunces`. Graisses utilisées : 400 (Regular) et 500 (Medium), plus
  l'italique 400 pour l'exergue de la section Vision.
- **Inter** — police de texte (navigation, paragraphes, étiquettes). Nom exact : `Inter`.
  Graisses : 400 et 500.

> **Si Site Creator ne propose pas Fraunces** dans son sélecteur de polices, deux substituts
> proches et disponibles partout : **Cormorant Garamond** ou **EB Garamond**. Garder Inter pour le
> texte dans tous les cas. (Les polices sont intégrées dans les fichiers HTML uniquement pour que
> les maquettes soient fidèles hors ligne — dans Site Creator, il suffit de choisir la police dans
> le menu, rien à téléverser.)

## Couleurs (codes hexadécimaux)

**Palette sombre**
| Usage | Hex |
|---|---|
| Fond | `#0E0E10` |
| Blocs en relief (film, portrait) | `#141417` |
| Texte principal | `#ECEAE3` |
| Texte secondaire | `#9A968C` |
| Filets / séparateurs | `#26262B` |
| Accent (croissant, filets, étiquettes) | `#C2A878` |

**Palette claire**
| Usage | Hex |
|---|---|
| Fond | `#F4F1EA` |
| Blocs en relief | `#FBF9F4` |
| Texte principal | `#15140F` |
| Texte secondaire | `#6B665C` |
| Filets / séparateurs | `#E3DCCE` |
| Accent | `#9C7A3A` |

Trois couleurs maximum par palette (fond, texte, accent), plus les neutres. **Aucun dégradé, aucun
effet métallique.** L'accent est un aplat mat.

## Éléments à surveiller lors de la reconstruction dans Site Creator

| Élément de la maquette | Difficulté | Substitut simple dans Site Creator |
|---|---|---|
| **Croissant** (motif de lune) | Dessiné en SVG dans la maquette | Téléverser le croissant comme **image** (extrait des PNG de logotype), ou utiliser le logotype choisi qui le contient déjà. |
| **Logotype** dans l'en-tête | Composé en HTML dans la maquette | Téléverser le **PNG transparent** de la direction retenue (`wordmark-w{n}-{dark/light}.png`). |
| **Apparition en fondu au défilement** | Petit script (amélioration progressive) | Utiliser l'animation « fondu / apparition » **native** de Site Creator par bloc — ou ne rien mettre. Le site reste parfaitement lisible sans animation. |
| **Lune du héros** | Image détourée (fond transparent) | Téléverser le PNG de lune fourni comme **image** dans le bloc héros. *(En attente de l'image définitive de la cliente ; le croissant graphique sert de provisoire.)* |
| **Formulaire de contact** | Statique dans la maquette | Reconstruire avec le **bloc formulaire natif** de Site Creator. Champs : `Nom`, `Email`, `Votre projet`. Sous le formulaire : bloc de coordonnées (email, téléphone, adresse). |
| **Portrait** | Rectangle généreux, sans recadrage | Bloc image simple. Ne pas recadrer en cercle, ne pas appliquer de filtre ni d'effet au survol. |
| **Chiffres 01–04 / 01–03** | Grands chiffres Fraunces | Simple texte en Fraunces. **Pas d'icônes** — les chiffres sont le motif. |

## Navigation et ancres

Menu collant, minimal : `Approche · Vision · Films · Équipe · Contact`.
Ancres : `#approche` · `#vision` (suivie de « Ce que nous faisons ») · `#films` (En développement) ·
`#equipe` · `#contact`.

## Coordonnées & domaine

- Domaine : **qamarfilmworks.com**
- Email affiché : **selou@qamarfilmworks.com**
- Téléphone : **07 68 01 90 96** · Adresse : **47 rue Vivienne, 75002 Paris, France**

## Structure de la page (une seule page, défilement)

Héros → Notre approche (01–04) → Vision → Ce que nous faisons (01–03) → En développement →
L'équipe → Contact → pied de page. **Aucune section ajoutée** au-delà du brief.

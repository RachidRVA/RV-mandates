# Guide de construction — Qamar Filmworks dans Infomaniak Site Creator

Ce guide vous accompagne pas à pas pour reconstruire le site à partir des maquettes, dans
**Infomaniak Site Creator**. Aucune compétence technique n'est requise. Comptez ~2 à 3 heures.

Gardez les maquettes ouvertes à côté pendant la construction : **tout le texte à copier s'y trouve
déjà, mot pour mot.** Ouvrez `mockup-dark.html` (ou `mockup-light.html`) dans votre navigateur — c'est
votre modèle visuel de référence.

---

## Avant de commencer — ce qu'il vous faut

- Votre compte **Infomaniak** avec **Site Creator** activé.
- Le domaine **qamarfilmworks.com** (chez Infomaniak).
- Le dossier de fichiers (ce dossier `qamar-filmworks/`), qui contient :
  - les images à téléverser (voir §4),
  - les maquettes (le modèle visuel),
  - `BUILD-NOTE.md` (les codes couleurs et polices, en résumé).

---

## 1. Créer le site

1. Dans Infomaniak, ouvrez **Site Creator** → **Créer un site**.
2. Choisissez un modèle **vierge / minimal** (le moins décoré possible — on part d'une page nue).
3. Langue du site : **Français**.
4. Structure : **une seule page** qui défile. On n'ajoute **pas** d'autres pages.

---

## 2. Réglages généraux (thème du site)

### Polices
Dans les réglages de **typographie** du thème :
- **Titres** → **Fraunces** (si absente de la liste : **Cormorant Garamond** ou **EB Garamond**).
- **Texte courant** → **Inter**.

### Couleurs
Choisissez **une** des deux palettes (celle que Sarah retient) et saisissez les codes exacts :

**Palette sombre**
| Rôle | Code |
|---|---|
| Fond du site | `#0E0E10` |
| Texte principal | `#ECEAE3` |
| Texte secondaire | `#9A968C` |
| Accent (traits, étiquettes) | `#C2A878` |

**Palette claire**
| Rôle | Code |
|---|---|
| Fond du site | `#F4F1EA` |
| Texte principal | `#15140F` |
| Texte secondaire | `#6B665C` |
| Accent | `#9C7A3A` |

> Règle d'or : **pas de dégradé, pas d'effet brillant/métallique.** L'accent est une couleur pleine.

---

## 3. La barre de navigation (menu collant)

1. Activez un **en-tête collant** (sticky) en haut de page.
2. À gauche : le **logotype** (image — voir §4). À droite : **5 liens** qui pointent vers les
   sections (liens d'ancre) :
   `Approche` · `Vision` · `Films` · `Équipe` · `Contact`.
3. Chaque lien renvoie à la section correspondante (dans Site Creator : « lien vers une section /
   ancre de la page »).

---

## 4. Les images à téléverser

Téléversez ces images dans la médiathèque de Site Creator :

| Image | Où | Remarque |
|---|---|---|
| **Logotype** | En-tête + pied de page | Utilisez le PNG de la direction retenue : `wordmark-w1/2/3-dark.png` (sur fond sombre) ou `…-light.png` (sur fond clair). Fond transparent. |
| **Lune (héros)** | Section héros, à droite | **Image définitive : NASA PIA00405** (domaine public, libre). Téléversez `PIA00405~large.jpg`, puis appliquez un filtre **noir & blanc / niveaux de gris**. Pas de halo, pas de reflet. *(La maquette montre une lune provisoire.)* |
| **Portrait de Sarah** | Section Équipe | `assets/portrait-sarah.jpg`. **Rectangle généreux**, sans recadrage en cercle, sans filtre, sans effet au survol. |

---

## 5. Les sections, dans l'ordre

Reproduisez ces sections de haut en bas. **Le texte exact est dans la maquette** — copiez-collez
depuis là. Ci-dessous : le type de bloc et ce qu'il contient.

1. **Héros** *(ancre : approche via le bouton)*
   - Petit sur-titre en majuscules espacées (couleur accent).
   - Grand titre (Fraunces) : « Une nouvelle génération de cinéastes ».
   - Sous-titre (Inter, gris).
   - Un **bouton / lien souligné** : « Découvrir notre approche → » qui renvoie à la section Approche.
   - À droite : l'**image de la lune**.

2. **Notre approche** *(ancre `Approche`)*
   - Chapô (Fraunces) : « Accompagner la nouvelle génération de cinéastes. »
   - **Quatre blocs numérotés 01 → 04**, séparés par un filet fin. Chaque bloc : le **grand chiffre**
     (Fraunces, couleur accent) + un titre + un paragraphe. **Pas d'icônes — les chiffres sont le
     motif.**

3. **Vision** *(ancre `Vision`)*
   - Petite étiquette « Vision ».
   - **Citation en exergue** (Fraunces *italique*, grand) : « De nouvelles voies pour le cinéma
     indépendant. »
   - Puis les paragraphes de texte.

4. **Ce que nous faisons**
   - Chapô (Fraunces).
   - **Trois blocs 01 → 03** côte à côte (sur mobile : l'un sous l'autre).

5. **En développement** *(ancre `Films`)*
   - Un **bloc encadré** (fin liseré) légèrement en relief.
   - Sur-titre « EN DÉVELOPPEMENT · PREMIER LONG MÉTRAGE », titre (Fraunces), paragraphe.

6. **L'équipe** *(ancre `Équipe`)*
   - **Deux colonnes** : à gauche le **portrait** (rectangle), à droite le nom
     « SARAH EL OUADILI », le rôle en italique, la biographie, et le lien « Parcours complet → »
     (à relier plus tard vers un PDF téléchargeable).

7. **Contact** *(ancre `Contact`)*
   - Titre (Fraunces) : « Parlons-en. » + une phrase d'introduction.
   - **Formulaire natif de Site Creator** — champs : **Nom**, **Email**, **Votre projet**, bouton
     **Envoyer**. Réglez la réception des messages vers `selou@qamarfilmworks.com`.
   - En dessous, un bloc de **coordonnées** : Email `selou@qamarfilmworks.com` · Téléphone
     `07 68 01 90 96` · Adresse `47 rue Vivienne, 75002 Paris, France`.

8. **Pied de page**
   - Logotype + « © 2026 Qamar Filmworks Production » + l'email.

> **N'ajoutez aucune autre section** (pas d'actualités, de partenaires, de témoignages, de
> newsletter). La sobriété fait partie du parti pris.

---

## 6. Animations

Optionnel : un **léger fondu à l'apparition** au défilement, si Site Creator le propose en natif
(par bloc). Sinon, **ne mettez rien** — le site reste parfaitement lisible sans animation. Aucune
autre animation.

---

## 7. Vérifier le rendu mobile

Dans Site Creator, basculez en **aperçu mobile** et vérifiez :
- rien ne dépasse sur les côtés (pas de défilement horizontal),
- les blocs numérotés et les colonnes passent bien **l'un sous l'autre**,
- le portrait et la lune restent nets,
- le menu reste accessible.

---

## 8. Domaine et mise en ligne

1. Reliez le domaine **qamarfilmworks.com** au site (réglages de domaine Infomaniak).
2. Vérifiez les liens du menu (chaque lien saute à la bonne section).
3. Vérifiez l'adresse email du formulaire et des coordonnées.
4. **Publiez.**

---

## 9. Modifier le site plus tard

Tout est éditable directement dans Site Creator : cliquez sur un texte pour le changer, sur une image
pour la remplacer. Pour rester fidèle au design, gardez : **les deux polices**, **les codes couleurs
ci-dessus**, la **sobriété** (pas de dégradé, pas d'effet brillant), et les **chiffres** à la place
d'icônes.

Besoin d'un contrôle final une fois le site construit ? Envoyez le lien — on fait une passe de
relecture visuelle ensemble.

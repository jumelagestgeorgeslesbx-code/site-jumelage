# Site du comité de jumelage Saint-Georges-lès-Baillargeaux – Denmead

Le site est hébergé gratuitement sur **GitHub Pages**. On le modifie avec **Pages CMS**, une interface web en français ou en anglais, sans aucun code.
Chaque enregistrement dans Pages CMS met le site en ligne automatiquement en 1 à 2 minutes.

---

## Partie 1 : mise en place (une seule fois, environ 20 minutes)

À faire par la personne la plus à l'aise avec l'informatique.

### 1. Créer un compte GitHub pour le comité
1. Allez sur https://github.com/signup et créez un compte, de préférence avec l'adresse e-mail du comité (par exemple `jumelage-stgeorges`).
2. Ce compte « appartient » au comité, ce qui évite de tout perdre quand le bureau change.

### 2. Créer le dépôt et y déposer les fichiers
1. Sur GitHub, cliquez sur **+** puis **New repository**.
2. Nom : `site-jumelage`. Visibilité : **Public** (obligatoire pour l'hébergement gratuit). Cliquez sur **Create repository**.
3. Cliquez sur le lien **uploading an existing file**.
4. Décompressez le fichier `site-jumelage.zip` sur votre ordinateur, puis glissez **tout le contenu** du dossier dans la page (`index.html`, les dossiers `content` et `images`, le fichier `.pages.yml`, etc.).
   - Les fichiers qui commencent par un point (`.pages.yml`, `.nojekyll`) sont parfois cachés. Sur Mac, appuyez sur Cmd + Maj + . pour les afficher. Sur Windows, cochez Affichage > Éléments masqués.
5. Cliquez sur **Commit changes**.

### 3. Mettre le site en ligne
1. Dans le dépôt, ouvrez **Settings** puis **Pages**.
2. Sous *Build and deployment*, choisissez Source : **Deploy from a branch**, Branch : **main**, dossier **/ (root)**, puis cliquez sur **Save**.
3. Une à deux minutes plus tard, l'adresse du site s'affiche en haut de cette page :
   `https://<nom-du-compte>.github.io/site-jumelage/`

### 4. Brancher l'interface d'édition
1. Allez sur https://app.pagescms.org et cliquez sur **Sign in with GitHub**. Connectez-vous avec le compte du comité.
2. Autorisez Pages CMS à accéder au dépôt `site-jumelage`.
3. Ouvrez le dépôt. Le menu de gauche affiche **Agenda, Galerie photos, Adhésion et tarifs, Présentation et contact, Nos communes**.

### 5. Donner l'accès aux autres membres du bureau
Choisissez l'une des deux solutions :
- **Avec un compte GitHub pour chacun** : dans le dépôt GitHub, ouvrez **Settings**, **Collaborators**, puis **Add people**. Chaque membre se connecte ensuite à app.pagescms.org avec son propre compte.
- **Sans compte GitHub** : dans Pages CMS, ouvrez **Settings** puis **Collaborators** et invitez la personne par e-mail. Elle reçoit un lien de connexion.

### 6. (Facultatif) Utiliser une adresse personnalisée
Pour avoir une adresse comme `jumelage-saintgeorges.fr` :
1. Achetez le nom de domaine chez OVH, Gandi, etc. (environ 10 € par an).
2. Sur GitHub, ouvrez **Settings**, **Pages**, **Custom domain**, saisissez le domaine et cliquez sur **Save**.
3. Chez le fournisseur du domaine, ajoutez les enregistrements DNS indiqués par GitHub dans sa documentation « Managing a custom domain for your GitHub Pages site ».
4. Cochez **Enforce HTTPS** une fois que l'option devient disponible.

---

## Partie 2 : mettre à jour le site (pour tous les membres)

1. Allez sur **https://app.pagescms.org** et connectez-vous.
2. Choisissez la rubrique à modifier dans le menu de gauche.
3. Modifiez, puis cliquez sur **Save** (Enregistrer).
4. Le site public est à jour 1 à 2 minutes plus tard. Rechargez la page pour voir le changement.

### Ce qu'on peut modifier

| Rubrique | Contenu |
|---|---|
| **Agenda** | Ajouter, modifier ou supprimer un rendez-vous (titre, date, lieu, description, photo). Les rendez-vous passés passent tout seuls dans « Rendez-vous passés ». |
| **Galerie photos** | Ajouter des photos avec une légende. La section Photos apparaît dès qu'il y a au moins une photo. |
| **Adhésion et tarifs** | Montants des cotisations, modalités de paiement, lien HelloAsso éventuel (un bouton « Adhérer en ligne » apparaît alors). |
| **Présentation et contact** | Texte d'accueil, présentation du comité, année du jumelage, président(e), e-mail, téléphone, adresse, liens Facebook et Denmead. |
| **Nos communes** | Descriptions, points clés et photo de chaque commune. |

### Conseils
- **Champs français et anglais** : remplissez les deux si possible. Si l'anglais est vide, le site affiche le texte français aux visiteurs anglophones, et inversement.
- **Date approximative** (« Mai 2027 ») : choisissez le 1er du mois dans le champ Date et écrivez « Mai 2027 » dans « Date affichée ».
- **Photos** : préférez des images de moins de 1 Mo, au format JPG. Elles sont plus rapides à charger sur téléphone.
- **Les champs vides sont masqués** : une information absente (président, téléphone…) n'apparaît simplement pas sur le site.
- **Erreur ou fausse manipulation** : GitHub garde l'historique de toutes les modifications. On peut toujours revenir en arrière depuis l'onglet « Commits » du dépôt.

---

## Pour les curieux : organisation des fichiers

```
index.html          la page et sa mise en forme
content/*.json      tout le contenu modifiable (lu par la page)
images/             les photos envoyées depuis Pages CMS
.pages.yml          la configuration de l'interface Pages CMS
.nojekyll           indique à GitHub Pages de publier les fichiers tels quels
```

Le formulaire d'adhésion ouvre la messagerie du visiteur avec une demande pré-remplie, adressée à l'e-mail du comité. Aucune donnée n'est stockée sur le site.

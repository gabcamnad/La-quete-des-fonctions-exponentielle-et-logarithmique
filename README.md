# Les Quêtes Exponentielles

Jeux de plateforme pour réviser les **fonctions exponentielles** et les **logarithmes** en secondaire 5 (Québec).

Deux jeux, mêmes notions :

| Jeu | Ambiance | Mondes |
|---|---|---|
| **Quête Exponentielle** | Plateformes en plein jour, musique 8-bit | Plaine des exposants · Vallée des paramètres · Volcan des situations · *Extension : montagne des logarithmes* |
| **Le Manoir Exponentiel** | Manoir hanté la nuit, sursauts sans violence (désactivables) | Cimetière des exposants · Manoir des paramètres · Crypte des situations · *Extension : marais des logarithmes* |

## Contenu pédagogique

- **Monde 1** : lois des exposants, exposants négatifs, nuls et fractionnaires, croissance ou décroissance
- **Monde 2** : asymptote, codomaine, ordonnée à l'origine, transformations, trouver la règle de *f*(*x*) = *a*(*c*)<sup>*b*(*x* − *h*)</sup> + *k*, forme canonique, inéquations exponentielles
- **Monde 3** : équations et inéquations exponentielles (aussi en situation), intérêts composés, dépréciation, demi-vie, doublement
- **Extension (Monde 4)** : évaluer un logarithme, forme exponentielle ↔ logarithmique, lois des logarithmes, changement de base, équations et inéquations logarithmiques, fonction logarithmique, réciproques (exponentielle ↔ logarithmique), forme canonique, trouver la règle d'une fonction logarithmique, problèmes (croissance, dépréciation, demi-vie, pH, magnitude d'un séisme)

Les questions sont générées au hasard à chaque partie. Chaque réponse est suivie d'une explication. Un bilan par notion s'affiche à la fin.

## Multijoueur : courses

Dans les deux modes, tous les joueurs reçoivent **les mêmes questions dans le même ordre**. Le premier qui bat le boss du monde choisi gagne.

- Bonne réponse : un cœur de plus et un **turbo** de 6 secondes
- Plus de cœurs : on repart aussitôt, avec **15 secondes de pénalité**
- Le chrono tourne aussi pendant les questions

### 2 joueurs sur le même écran

Sur l'écran titre, clique sur **2 joueurs · même écran** sous le jeu choisi, puis choisis un monde. L'écran se partage en deux.

| Joueur | Bouger | Sauter | Répondre |
|---|---|---|---|
| Joueur 1 (en haut) | A, D | W | 1, 2, 3, 4 |
| Joueur 2 (en bas) | ←, → | ↑ | 7, 8, 9, 0 |

On peut aussi cliquer sur les réponses. Ce mode fonctionne avec le lien GitHub Pages et avec le fichier hors ligne. Il ne fonctionne pas si on ouvre `index.html` directement depuis un dossier de l'ordinateur : dans ce cas, utilise `quetes-exponentielles-hors-ligne.html`.

### Course en ligne (chacun sur son appareil)

1. Dans le jeu, clique sur **Course en ligne (multijoueur)** et écris ton nom.
2. Un joueur clique sur **Créer** et reçoit un code de 4 lettres. Il choisit le monde.
3. Les autres tapent le code et cliquent sur **Rejoindre** (8 joueurs au maximum, dans le même jeu).
4. L'hôte clique sur **Lancer la course**. Chacun voit les autres avancer en direct (silhouettes et classement).

Il faut une connexion Internet. Chaque appareil essaie deux chemins en même temps et garde le premier qui fonctionne : un **relais Internet** (serveurs MQTT publics et gratuits, par connexion web sécurisée, qui passent sur la plupart des réseaux d'école) et une **connexion directe** entre les appareils (PeerJS). Une fois connecté, le jeu affiche « relais Internet » ou « connexion directe ».

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Écran titre : choix du jeu |
| `quete-exponentielle.html` | Jeu classique |
| `manoir-exponentiel.html` | Jeu version horreur |
| `quetes-exponentielles-hors-ligne.html` | Les deux jeux et l'écran titre dans **un seul fichier**, à copier sur une clé USB ou à télécharger pour jouer sans Internet |

Aucune installation n'est nécessaire : chaque fichier est autonome (HTML, CSS et JavaScript dans le même fichier).

## Publier avec GitHub Pages

1. Dépose tous les fichiers à la racine du dépôt (pas dans un sous-dossier).
2. Dans le dépôt, va dans **Settings → Pages**.
3. Sous *Build and deployment*, choisis **Deploy from a branch**, la branche **main** et le dossier **/ (root)**, puis **Save**.
4. Après une minute ou deux, le lien apparaît en haut de la page : `https://<ton-nom-utilisateur>.github.io/<nom-du-depot>/`

Partage ce lien dans Classroom avec **Ajouter → Lien**.

## Commandes

- Clavier : ← → pour bouger, Espace ou ↑ pour sauter, 1 à 4 pour répondre, Échap pour la pause
- Téléphone et tablette : boutons à l'écran
- Réglages sur l'écran d'accueil de chaque jeu : temps limite par question, musique, effets sonores, sursauts (version horreur)
- Le multijoueur utilise les librairies [MQTT.js](https://github.com/mqttjs/MQTT.js) et [PeerJS](https://peerjs.com/) (licence MIT), chargées seulement quand on ouvre la course en ligne

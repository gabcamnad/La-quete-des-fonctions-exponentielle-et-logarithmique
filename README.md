# Les Quêtes Mathématiques

Quatre jeux de plateforme pour réviser les mathématiques de secondaire 5 (Québec), réunis sur un même écran titre.

| Jeu | Notions | Ambiance |
|---|---|---|
| **Quête Exponentielle** | Fonctions exponentielles, extension sur les logarithmes | Plateformes en plein jour |
| **Le Manoir Exponentiel** | Mêmes notions | Manoir hanté la nuit, sursauts sans violence (désactivables) |
| **Quête Trigonométrique** | Cercle trigonométrique, identités, sinus, cosinus, tangente | Plateformes en plein jour, bord de mer |
| **Quête Trigonométrique des Fêtes** | Mêmes notions | Neige, cadeaux et chants de Noël en 8 bits |

## Contenu pédagogique : fonctions exponentielles et logarithmiques

- **Monde 1** : lois des exposants, exposants négatifs, nuls et fractionnaires, croissance ou décroissance
- **Monde 2** : asymptote, codomaine, ordonnée à l'origine, transformations, trouver la règle de *f*(*x*) = *a*(*c*)<sup>*b*(*x* − *h*)</sup> + *k*, forme canonique, inéquations exponentielles
- **Monde 3** : équations et inéquations exponentielles (aussi en situation), intérêts composés, dépréciation, demi-vie, doublement
- **Extension (Monde 4)** : évaluer un logarithme, forme exponentielle ↔ logarithmique, lois des logarithmes, changement de base, équations et inéquations logarithmiques, fonction logarithmique, réciproques (exponentielle ↔ logarithmique), forme canonique, trouver la règle d'une fonction logarithmique, problèmes (croissance, dépréciation, demi-vie, pH, magnitude d'un séisme)

Les questions sont générées au hasard à chaque partie. Chaque réponse est suivie d'une explication. Un bilan par notion s'affiche à la fin.

## Contenu pédagogique : trigonométrie

- **Monde 1 – Cercle trigonométrique** : degrés ↔ radians, point trigonométrique *P*(θ), valeurs exactes, tangente, signes selon le quadrant, trouver θ à partir des coordonnées, longueur d'arc, angles coterminaux
- **Monde 2 – Identités** : sec, cosec et cotan, identités de Pythagore, calculer une valeur avec une identité et le quadrant, simplifier, reconnaître et démontrer une identité
- **Monde 3 – Sinus et cosinus** : période, codomaine, tracer la courbe (choix de graphiques), rechercher la règle de *f*(*x*) = *a* sin(*b*(*x* − *h*)) + *k* à partir d'un graphique ou d'un maximum et d'un minimum, transformations, liens entre sinus et cosinus
- **Monde 4 – Équations et inéquations** : équations sur [0, 2π], solution générale, équations de la forme *a* sin *x* + *k* = *c* et sin 2*x* = *c*, inéquations, problèmes (grande roue, temps passé au-dessus d'une hauteur, température d'une serre)
- **Monde 5 – Tangente** : période, asymptotes, point d'inflexion, variation, équations, solution générale, inéquations, tracer la courbe, rechercher la règle, problème du projecteur

Les questions sont générées au hasard à chaque partie. Chaque réponse est suivie d'une explication. Un bilan par notion s'affiche à la fin. L'aide-mémoire est accessible dans le menu pause.

## Pièces et boutique de skins

- Pièces à ramasser dans chaque niveau (+1), blocs à casser (+1) et bonnes réponses (+5)
- Toutes les 25 pièces gagnées dans un monde : +1 cœur
- Jeux exponentiels : 18 skins partagés entre la Quête et le Manoir (dont une tortue et des skins d'Halloween)
- Jeux de trigonométrie : pièces partagées entre les deux versions, 10 skins par version
- Chaque skin (sauf le premier) donne un **pouvoir**, actif aussi en course : double saut, vitesse, super saut, planeur, aimant à pièces, pièces ×2, bouclier, gel des ennemis, cœur bonus, seconde chance, sortilège (un mauvais choix disparaît), +50 % d'XP, etc. Le pouvoir est indiqué dans la boutique et dans le menu pause.
- Tout est gardé sur l'appareil; en course, les adversaires voient ton skin

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

On peut aussi cliquer sur les réponses. Ce mode fonctionne avec le lien GitHub Pages et avec le fichier hors ligne. Il ne fonctionne pas si on ouvre `index.html` directement depuis un dossier de l'ordinateur : dans ce cas, utilise `quetes-mathematiques-hors-ligne.html`.

### Course en ligne (chacun sur son appareil)

1. Dans le jeu, clique sur **Course en ligne (multijoueur)** et écris ton nom.
2. Un joueur clique sur **Créer** et reçoit un code de 4 lettres. Il choisit le monde.
3. Les autres tapent le code et cliquent sur **Rejoindre** (8 joueurs au maximum, tous dans le même jeu).
4. L'hôte clique sur **Lancer la course**. Chacun voit les autres avancer en direct (silhouettes et classement).

Il faut une connexion Internet. Chaque appareil essaie deux chemins en même temps et garde le premier qui fonctionne : un **relais Internet** (serveurs MQTT publics et gratuits, par connexion web sécurisée, qui passent sur la plupart des réseaux d'école) et une **connexion directe** entre les appareils (PeerJS). Une fois connecté, le jeu affiche « relais Internet » ou « connexion directe ».

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Écran titre : choix parmi les 4 jeux |
| `quete-exponentielle.html` | Quête Exponentielle |
| `manoir-exponentiel.html` | Le Manoir Exponentiel |
| `quete-trigonometrique.html` | Quête Trigonométrique |
| `quete-trigonometrique-fetes.html` | Quête Trigonométrique des Fêtes |
| `quetes-mathematiques-hors-ligne.html` | Les 4 jeux et l'écran titre dans **un seul fichier**, pour jouer sans Internet |

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
- Musique du temps des fêtes : arrangements 8 bits de chants du domaine public
- Le multijoueur utilise les librairies [MQTT.js](https://github.com/mqttjs/MQTT.js) et [PeerJS](https://peerjs.com/) (licence MIT), chargées seulement quand on ouvre la course en ligne

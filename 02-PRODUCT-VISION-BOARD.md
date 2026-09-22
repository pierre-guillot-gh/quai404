# Product Vision Board — QUAI 404

---

## 🔭 VISION
> *Pourquoi créer ce produit ? Quel changement positif doit-il apporter ?*

### « Plus personne ne monte dans le mauvais train. »

Aujourd'hui, le réseau ne manque pas d'information : il en produit toujours autant.
Elle est simplement devenue **fausse — sans le dire**. Panneaux, annonces et app
officielle continuent d'affirmer avec la même assurance qu'hier.

Le changement que nous apportons : **rendre la fiabilité de l'information visible.**
Le voyageur cesse de deviner et redevient capable de décider, même pendant que
le système se trompe.

> *Une information honnêtement incertaine vaut mieux qu'une information faussement certaine.*

---

## 🎯 CIBLE
> *Quel segment ? Quels utilisateurs et clients ?*

**Marché** — mobilité ferroviaire suisse en situation de perturbation majeure.
~1,3 M de voyageurs/jour sur le réseau CFF.

**Client** *(qui paie)* : les CFF.
**Utilisateur** *(qui s'en sert)* : le voyageur.

### Persona principal — Nadia Berger, 34 ans
Consultante, Lausanne → Berne, rendez-vous client à 10h00.
App CFF utilisée par réflexe, pas experte du réseau.

**Son moment : 08:47, voie 3.** Un train est devant elle. Le panneau dit « Berne »,
l'annonce sonore dit autre chose, son app une troisième. **Les portes ferment dans 40 secondes.**

> **« Est-ce que je monte dans CELUI-LÀ ? »**

**Contributeurs** — les mêmes personnes, un moment plus tard : le voyageur
déjà à bord, qui lui sait où il se trouve réellement.

**Hors périmètre v1** — voyageurs PMR · sans smartphone · groupes · non-francophones.

---

## ❗ BESOINS
> *Quel problème résolu ? Priorisés, le plus important en premier.*

### 1️⃣ Savoir si **ce train-là, physiquement devant moi**, va où je vais
Pas un horaire théorique. Un verdict sur l'objet réel qui est à quai, maintenant.

### 2️⃣ Pouvoir arbitrer un risque dont le coût est asymétrique

| | Si juste | Si faux |
|---|---|---|
| **Je monte** | j'arrive à l'heure | **2 h perdues**, RDV manqué |
| **J'attends** | je perds 8 min | je perds 8 min |

Rien aujourd'hui n'aide Nadia à peser ces deux branches : l'app officielle les
présente **avec la même assurance**.

### 3️⃣ Savoir ce que le système **ne sait pas**
Un « je ne sais pas » explicite est actionnable. Une affirmation fausse ne l'est pas.

### 4️⃣ Connaître la **source** et la **fraîcheur** de l'information
Qui le dit, et depuis quand ? Sans ça, aucune information ne peut être pondérée.

### 5️⃣ Disposer d'une **alternative chiffrée**
Pas « consultez les horaires », mais « voie 7, dans 11 min, confiance 84 % ».

---

## 📦 PRODUIT
> *Quel produit ? 3 à 5 caractéristiques distinctives ? Réalisable ? Proposition de valeur ? Critères de succès ?*

**QUAI 404** — application web mobile-first, utilisable en 40 secondes sur un quai.
Un écran, une décision, un seul moment du parcours.

### Proposition de valeur
> **Quai 404 vous dit si le train devant vous va vraiment où vous allez —
> et vous dit franchement quand il l'ignore.**

### Les 5 caractéristiques distinctives

| # | Caractéristique | Pourquoi personne d'autre ne le fait |
|---|---|---|
| **1** | **Verdict sur le train physique**, pas sur l'horaire | tout le marché raisonne en horaires théoriques |
| **2** | **Trois états assumés** : ✅ Confirmé · ⛔ Infirmé · ❓ Inconnu | le système officiel n'a pas d'état « inconnu » |
| **3** | **Source + fraîcheur + niveau de confiance** sur chaque affirmation | la donnée système est explicitement marquée *non vérifiée* |
| **4** | **Boucle terrain** : confirmer en 1 tap une fois à bord | chaque voyageur sauvé devient le capteur du suivant |
| **5** | **Recommandation d'action** avec alternative confirmée | on ne livre pas de la donnée, on livre une décision |

### Réalisable ?
**Oui, et c'est le point fort :** le produit **ne dépend pas de la réparation du bug**.
Il ne consomme la donnée système que comme un signal parmi d'autres, dégradé au rang
de « non vérifié ». Techniquement : une app web, un backend de collecte, une règle de
consensus. Aucune intégration critique dans les systèmes de sécurité ferroviaire.
**Le prototype tourne déjà.**

### Ce que le produit n'est PAS
❌ un remplacement de l'app CFF · ❌ un planificateur d'itinéraire ·
❌ un dashboard d'exploitation · ❌ une correction du bug

### Critères de succès

| Critère | Cible |
|---|---|
| ⭐ **North Star — voyageurs montant dans le bon train** | **> 90 %** *(baseline crise ≈ 50 %)* |
| Temps de décision sur le quai | < 15 s |
| Taux de contribution | ≥ 5 % des voyageurs confirment |
| Couverture réseau | ≥ 70 % des trains actifs avec confirmation < 10 min |

### Concurrence — les alternatives actuelles de Nadia
App CFF officielle · panneaux · annonces sonores · agent de gare saturé · X/Twitter.
Toutes partagent la **même source corrompue**, ou sont inexploitables en 40 secondes.

> Le concurrent réel, c'est **« demander à son voisin de quai »**. Ça marche déjà.
> **Quai 404, c'est cette pratique qui passe à l'échelle.**

---

## 💼 OBJECTIFS BUSINESS
> *Quels bénéfices pour les CFF ? Priorisés, le plus important en premier.*

### 1️⃣ Réduire le nombre de voyageurs mal aiguillés
C'est le coût dominant de la crise : chaque erreur d'embarquement génère 2 h de
trajet parasite, une réclamation, un appel et une place occupée pour rien.
*Mesure : % de bons embarquements.*

### 2️⃣ Reconstruire la confiance par l'honnêteté calibrée
La réputation suisse de fiabilité est l'actif le plus précieux des CFF. Un canal qui
admet ses limites la protège mieux qu'un canal qui se trompe avec aplomb.
*Mesure : NPS pendant et après crise.*

### 3️⃣ Désengorger le terrain
Agents de gare et Rail Service 0848 absorbent aujourd'hui toute la demande
d'information. L'auto-service la fait chuter.
*Mesure : volume d'appels, longueur des files en gare.*

### 4️⃣ Constituer gratuitement une carte de vérité terrain
Les confirmations des voyageurs produisent une vue du réseau réel, immédiatement
réutilisable par l'exploitation — là où les capteurs système sont corrompus.
*Mesure : nombre de trains localisés par heure.*

### 5️⃣ Réduire les indemnisations
Moins d'erreurs d'aiguillage, moins de dossiers. Et les confirmations horodatées
fournissent la preuve que le système corrompu ne peut plus produire.
*Mesure : CHF de réclamations évitées.*

---

## 🚀 Roadmap post-hackathon *(à citer, pas à construire)*

**v2** — les agents CFF, à bord comme en gare, comme source prioritaire · **v3** — console d'arbitrage
pour l'information voyageurs · **v4** — certificat de perturbation automatique pour
l'indemnisation · **v5** — hors-crise : détection précoce d'anomalies par les pendulaires.

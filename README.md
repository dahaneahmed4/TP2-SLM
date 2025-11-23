TP N°2 : Commandabilité et Observabilité d'un Bras Manipulateur 2-DOF

Université des Sciences et de la Technologie Houari Boumediene (USTHB) Faculté d'Électronique et d'Informatique Département : Automatique

Niveau : Master 1 - Automatique et Informatique Industrielle (AII)

Module : Systèmes Linéaires Multivariables (SLM)

Année Universitaire : 2025/2026

BINOM: DAHANE AHMED LAMINE & RAMZI MAMOU

📋 Description du Projet

Ce dépôt contient la solution complète et le compte-rendu interactif du TP N°2 concernant l'analyse et la commande d'un bras manipulateur à deux degrés de liberté (2-DOF).

L'objectif principal est d'étudier les propriétés structurelles d'un système multivariable (MIMO) linéarisé et de concevoir une loi de commande par retour d'état pour améliorer ses performances dynamiques.

🚀 Contenu du Dépôt

index.html : Le fichier principal. Il s'agit d'un compte-rendu interactif généré en HTML5. Il contient :

Le code MATLAB complet et commenté.

Les explications théoriques détaillées (analyse spectrale, critères de Kalman).

Des simulations graphiques interactives (réponses indicielles en boucle ouverte et fermée) générées avec Plotly.js.

🛠️ Travail Réalisé

1. Modélisation

Le système est modélisé par une représentation d'état continue $\dot{x} = Ax + Bu$, avec :

4 États ($x$) : Positions angulaires ($\theta_1, \theta_2$) et vitesses angulaires ($\dot{\theta}_1, \dot{\theta}_2$).

2 Entrées ($u$) : Couples moteurs appliqués aux articulations.

2 Sorties ($y$) : Positions angulaires mesurées.

2. Analyse des Propriétés

Stabilité : Calcul des valeurs propres de la matrice $A$. Le système est identifié comme stable mais fortement oscillant (sous-amorti).

Commandabilité : Vérification du rang de la matrice de commandabilité $\mathcal{C}$. Le système est complètement commandable (rang = 4).

Observabilité : Vérification du rang de la matrice d'observabilité $\mathcal{O}$. Le système est complètement observable (rang = 4).

3. Synthèse de la Commande

Mise en œuvre d'une commande par retour d'état $u = -Kx + N \cdot r$ :

Placement de Pôles : Calcul du gain $K$ pour imposer des pôles réels (rapidité) et complexes conjugués (amortissement) : $\{-3, -3.5, -4 \pm 2j\}$.

Pré-compensation : Calcul du gain de préréglage $N$ pour assurer une erreur statique nulle (suivi de consigne parfait).

📊 Résultats

Les simulations montrent que la commande proposée transforme radicalement la dynamique du robot :

Suppression des oscillations mécaniques.

Réduction du temps de réponse (système plus rapide).

Découplage effectif des axes.

Précision parfaite en régime permanent.

💻 Comment visualiser le rapport ?

Option 1 : Via GitHub Pages (Recommandé)

Si "GitHub Pages" est activé sur ce dépôt :

Cliquez sur le lien de déploiement dans la section "Environments" ou dans la description du dépôt (généralement https://votre-username.github.io/nom-du-repo/).

Option 2 : En local

Clonez ce dépôt ou téléchargez le fichier index.html.

Ouvrez simplement index.html avec n'importe quel navigateur web moderne (Chrome, Firefox, Edge).

Auteur : DAHANE AHMED LAMINE & RAMZI MAMOU

Encadrant : LYDIA

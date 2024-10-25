# wander
Voici un README détaillant les comportements implémentés dans votre projet :

---

# Projet de Simulation de Comportements de Véhicules avec p5.js

Ce projet utilise la bibliothèque **p5.js** pour simuler le comportement autonome de véhicules dans un espace virtuel. Les véhicules adoptent différents comportements basés sur des algorithmes de dynamique comportementale, simulant des mouvements réalistes et adaptatifs.

## Contenu du Projet

- **index.html** : Le fichier HTML principal qui charge les bibliothèques et scripts nécessaires.
- **jsconfig.json** : Configuration de compilation pour le support ES6.
- **style.css** : Styles de base pour le rendu du canvas.
- **sketch.js** : Script principal qui initialise les véhicules et gère le canvas.
- **vehicle.js** : Définit la classe `Vehicle` et implémente divers comportements de déplacement.

## Comportements Implémentés

1. **Errance (Wander)** :  
   Le véhicule se déplace de manière aléatoire avec une direction changeante, suivant un point cible qui oscille autour d'un cercle devant lui. Ce comportement permet de simuler un mouvement organique, créant une trajectoire fluide et imprévisible.

2. **Recherche (Seek)** :  
   Ce comportement oriente le véhicule vers une cible spécifique. Le véhicule ajuste sa vitesse pour pointer directement vers la cible, en appliquant une force de direction qui lui permet de suivre un chemin linéaire jusqu'à celle-ci.

3. **Évitement (Evade)** :  
   Le véhicule peut échapper à un autre véhicule en inversant sa trajectoire. Cet algorithme anticipe la position future de l'objet à éviter, permettant au véhicule de prendre une direction opposée pour esquiver efficacement.

4. **Pourchasse (Pursue)** :  
   Semblable à la recherche, la poursuite prend en compte le déplacement de la cible pour prédire sa position future, permettant au véhicule de maintenir une trajectoire calculée en direction de la cible en mouvement.

5. **Arrivée (Arrive)** :  
   Lorsqu'un véhicule s'approche de sa cible, il réduit progressivement sa vitesse pour arriver en douceur, ce qui évite des arrêts brusques et ajoute un réalisme au comportement en simulant une décélération naturelle.

6. **Fuite (Flee)** :  
   Le comportement de fuite est l'inverse de la recherche. Ici, le véhicule s'éloigne activement d'un point cible indésirable, simulant une réaction de peur ou de répulsion vis-à-vis d'une menace.

7. **Gestion des Bords (Edges)** :  
   Lorsque le véhicule atteint les limites du canvas, il réapparaît de l'autre côté, créant un effet de boucle continue et assurant qu'il reste actif et visible dans l'espace de simulation.

## Instructions d'Utilisation

1. **Ouvrir `index.html`** dans un navigateur compatible.
2. Le sketch génère un canvas où un ou plusieurs véhicules adoptent des comportements dynamiques et interactifs.

---

Ce fichier README donne un aperçu complet des comportements de simulation inclus dans le projet.

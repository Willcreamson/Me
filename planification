### Roadmap projet par projet : quoi construire, sur quoi se baser, avec quels outils

Tu as raison : une roadmap sans projet concret + référence de départ + critères de réussite laisse un trou entre la théorie et la pratique. Voici les projets clés de la roadmap, détaillés comme des mini-spécifications d’ingénierie.

### Projet 1 — GridWorld + Value Iteration (Mois 1)

![reinforcement learning - calculating the value of a state in an optimal policy analytically and iteratively - Artificial Intelligence Stack Exchange](https://images.openai.com/static-rsc-4/C4Mia8-ZJ5LTxEiLQfxd5l4o-Q-M1Qw1OJKCfdZg18eCKKB29dQD1Fs6ushTM1cYq0udvRuk5XKaU48ATqGuhDNEGRE94D4Z52MUnr-Rk7kCG-Ydal51eihoTXZ-g506GjWAmfx6w4FrIpyHtFDVuMVclOl8cjh2maVT2e6rDISJo0fhzAB4CcWnScJqv3TO?purpose=fullsize)

Ce qu’est un GridWorld : un monde discret en grille (ex. 4×4 ou 10×10). Chaque cellule est un état. L’agent peut faire des actions (haut, bas, gauche, droite). Certaines cases donnent une récompense positive, négative ou terminale.

À lire avant de coder

1. Reinforcement Learning: An Introduction — chapitres 3 et 4 (finite MDPs, dynamic programming).

2. OpenAI Spinning Up — sections d’introduction aux MDP/RL pour le vocabulaire : Spinning Up in Deep RL .

Ce que le projet doit faire

Implémenter Value Iteration et Policy Iteration sans Gymnasium ni SB3.

Représentation minimale :

Critères de réussite :

1. la fonction de valeur converge (delta < 1e-6),

2. la politique optimale atteint la cible,

3. tu peux afficher une carte de chaleur des valeurs et les flèches de la politique.

Outils autorisés

* Python 3.11+

* NumPy

* Matplotlib (visualisation)

Pourquoi ce projet est important

Tu apprends à définir explicitement un MDP : états, actions, transitions, récompenses, politique. C’est la brique conceptuelle de toute la suite.

### Projet 2 — Q-Learning from scratch (Mois 1-2)

![Aprendizado por Reforço #4— Gym. A caixa de areia da Inteligência… | by Enzo Cardeal Neves | Turing Talks | Medium](https://images.openai.com/static-rsc-4/P942EhxwASW3etIsZqxCc_TRM-M6PaXq1JzglAwij4Nnx1HPFMFAff26PsAbwCDzqyycN0CHNzyni305su7TF5uKq_Utcjp_UZWpgqr0tEeTYax-QQOOwD3fMM76xD_X3jTHWjkWqtbceygyxWNkdG7d9qbaXppg5fGZNLH_B-FsubGdSsvWQG88H5f-5-KJ?purpose=fullsize)

Ce qu’est Q-Learning : apprendre une valeur d’action Q(s,a) à partir de l’expérience, sans connaître le modèle de transition.

Références

* Reinforcement Learning: An Introduction — chapitres 5 et 6 (Monte Carlo, TD, SARSA, Q-Learning).

* Gymnasium docs — uniquement pour les environnements : Gymnasium .

Ce que le projet doit faire

1. Commencer sur FrozenLake-v1 (petit espace d’états).

2. Implémenter toi-même la boucle d’apprentissage :

Puis comparer avec Taxi-v3.

Critères de réussite :

* courbe de récompense moyenne croissante,

* taux de succès stable sur FrozenLake,

* tu peux expliquer epsilon-greedy et l’effet de alpha/gamma.

Outils

* Gymnasium

* NumPy

* Matplotlib

### Projet 3 — PPO sur CartPole/LunarLander (Mois 2)

![Proximal Policy Optimization (PPO) — How Do You Learn 0.0.1 documentation](https://images.openai.com/static-rsc-4/7NmeKrqBoAxZzKmELazUDjlS1RXZ_q7YVCLIkd9mu9rJIewW5CXAvhu-Bn4wbptlBiyVQvZmqN4OGPWUZpzZ2n_ZIzsKRFH2w1l8CWmMXCjUZdGeQNdXCtp_t8hC3AbI5LxUZpArm1Yoqo0NAurFYXRykHQ2mCLVDmCibC-7QyYpodbzVQMbQZsoTu806-bp?purpose=fullsize)

Ici tu arrêtes de tout coder à la main et tu apprends à utiliser un framework RL moderne.

Références

* OpenAI Spinning Up — PPO / Policy Gradient .

* Stable-Baselines3 docs — PPO : Stable-Baselines3 documentation .

Ce que le projet doit faire

1. Entraîner PPO sur CartPole-v1.

2. Sauvegarder les checkpoints.

3. Tracer les récompenses et le temps d’entraînement.

4. Puis passer à LunarLander-v2/v3.

Critères de réussite :

* CartPole résolu de manière stable,

* pipeline reproductible (seed fixée),

* README expliquant les hyperparamètres principaux.

Outils

* Stable-Baselines3

* PyTorch (via SB3)

* TensorBoard (optionnel)

### Projet 4 — Path Planner (Dijkstra + A*) (Mois 3)

![Generate Code for Path Planning Using Hybrid A Star - MATLAB & Simulink](https://images.openai.com/static-rsc-4/_Tt3HVjyulZFQJIxvJCGB6AWHXEw9bBNUdk6waMxpobl9FtzmLTpiS0o-0n1WurbHm58uqSScERL_QTjv4u6lYgPsGljk_nb_GFZrKzbBeWll8WkMzBJ4ZFTKV0EGsB3qF0oGTsZ7zpYdK9hJMYCqOMrTjJ4vOEML8s_tAjUbru3EC7HAxCaQBRujbdOS5t_?purpose=fullsize)

Ce projet est central pour la robotique et la navigation autonome.

Références

* Algorithms — graphes, shortest paths.

* Introduction à A* : Red Blob Games — A* Introduction .

Ce que le projet doit faire

Entrée :

Sortie :

Fonctionnalités :

1. Dijkstra.

2. A* avec heuristique Manhattan.

3. Visualisation du front de recherche.

4. Comparaison du nombre de nœuds explorés.

Critères de réussite :

* A* trouve le même coût optimal que Dijkstra,

* moins de nœuds explorés,

* benchmarks sur plusieurs cartes.

Outils

* Python + heapq

* Optionnel : Pygame ou Matplotlib animation

### Projet 5 — Kalman Filter 2D (Mois 5)

![An Application of the Kalman Filter Recursive Algorithm to Estimate the Gaussian Errors by Minimizing the Symmetric Loss Function | MDPI](https://images.openai.com/static-rsc-4/mex1jdLFNUGkQO1QZLpn_GuoqqARypShDYkBxXqwwFnBp7yT3vrvegygXNiLjYFw4MYXH-tOyTNh92zijqNIE3LG4s-3pyCiNx9f8j0qqbAj53rO-DhPqhUXsb-FLuG5uKEHj2YkW6frtLTVDymZ-giBIAM57eP5MGtWBESPEiWQyb45Usd4rsYhK9HbvC8a?purpose=fullsize)

Ce que c’est : un estimateur d’état qui combine un modèle de mouvement et des mesures bruitées.

Références

* KalmanFilter.net — intuition + équations .

* Tutoriel Python : FilterPy documentation (tu peux t’en inspirer sans utiliser la librairie au début).

Ce que le projet doit faire

Simuler :

* une trajectoire réelle (ground truth),

* des mesures GPS bruitées,

* un modèle vitesse constante.

Implémenter :

1. prédiction x = F x, P = F P Fᵀ + Q ;

2. mise à jour K = P Hᵀ (H P Hᵀ + R)⁻¹, etc.

Critères de réussite :

* la trajectoire filtrée est visiblement meilleure que les mesures brutes,

* tu peux expliquer le rôle de Q et R.

Outils

* NumPy

* Matplotlib

* Optionnel : FilterPy pour validation

### Projet 6 — ROS2 Mini Navigation Stack (Mois 7)

![ROS 2 Navigation — ROS 2 workshop documentation](https://images.openai.com/static-rsc-4/RqoMBY63PR3Q9svdP2HuZaDI_7t6P5nIU9IdibDLh-I1ak7xgV53gmX3eum03RbdyS1kDhAtae4tEi6vEF4z1IvYAYa9oG2UxoG9gHfAlqQYKLIpgDaXTNNx32PA-sXy_LFQj4ql8iGzPMwMXOd8SwytUAYccxX1RaKodIm2PET3LlglneLis0f7P_hFA24i?purpose=fullsize)

Ce qu’est ROS2 : un middleware robotique basé sur des nœuds qui communiquent via des topics/services/actions.

Références

* ROS2 Humble tutorials : ROS2 Humble Tutorials .

* Gazebo docs : Gazebo documentation .

Ce que le projet doit faire

Nœuds minimum :

| Nœud              | Rôle                   |
| ----------------- | ---------------------- |
| map_server        | publie la carte        |
| localization_node | publie la pose estimée |
| planner_node      | calcule un chemin A*   |
| controller_node   | suit le chemin         |

Critères de réussite :

* le robot atteint une cible dans Gazebo,

* les topics sont visibles via `ros2 topic list`,

* un launch file démarre tout le système.

Outils

* ROS2 Humble ou Iron

* Gazebo

* RViz2

### Projet 7 — Autonomous Navigation Simulator (Mois 8-9)

![Determining optimum assembly zone for modular reconfigurable robots using multi-objective genetic algorithm | Scientific Reports](https://images.openai.com/static-rsc-4/hPDdw_TNECaaFzBpshMNgC-Ye3ulPrxyU1f2XibOCbwoL_RemNiG5fuaQfMtQmxPwpRFX0wDRSxCWsZ92aJBXVdB8irYKiKKJHnwIa39r_QDaI9b2GyAvn6yE5ec75yiu4aY0cGVocEdBXa1pAq1U42wCaDYCqzMfV4P0Zwk4JmHaCwLE6HbNrFbJMAPhWTn?purpose=fullsize)

Le projet portfolio principal. Il assemble tout le pipeline.

Architecture cible

Fonctionnalités minimales :

1. carte 2D,

2. obstacles statiques,

3. pose bruitée,

4. Kalman filter,

5. A* replanné si obstacle ajouté,

6. visualisation temps réel.

Bonus :

* obstacles dynamiques,

* remplacement du planner par PPO,

* multi-agent simple.

Critères de réussite :

* démo vidéo < 2 min,

* README avec architecture,

* diagramme des nœuds/threads,

* benchmarks (temps de planification, taux d’échec, longueur moyenne de trajectoire).

Comment choisir la référence “source de vérité” pour chaque projet

Règle simple :

| Projet         | Source de vérité principale |
| -------------- | --------------------------- |
| GridWorld / DP | Sutton & Barto chap. 3-4    |
| Q-Learning     | Sutton & Barto chap. 5-6    |
| PPO            | Spinning Up + SB3 docs      |
| Dijkstra / A*  | Sedgewick + Red Blob Games  |
| Kalman         | KalmanFilter.net            |
| ROS2 / Gazebo  | ROS2 Tutorials officiels    |

Important : pour chaque projet, n’utilise qu’une source principale au début. Le but est d’éviter la dispersion entre 10 blogs contradictoires.

Piège à éviter (très fréquent chez les ingénieurs expérimentés)

Ne commence pas par ROS2, Gazebo ou un gros simulateur.

Fais d’abord :

1. GridWorld + Value Iteration

2. Q-Learning from scratch

3. A*

4. Kalman 2D

Ces quatre projets créent le socle mental. Ensuite ROS2 devient un problème d’intégration logicielle, pas un problème de compréhension algorithmique.

Plan hebdomadaire réaliste (si tu travailles déjà)

| Jour     | Temps | Type de travail                         |
| -------- | ----- | --------------------------------------- |
| Lundi    | 1 h   | lecture ciblée (1 section du livre/doc) |
| Mardi    | 1 h   | implémentation d’une fonction clé       |
| Mercredi | 1 h   | tests + visualisation                   |
| Jeudi    | 1 h   | refactor + README                       |
| Samedi   | 3-4 h | intégration / debugging / benchmark     |
| Dimanche | 1 h   | rétro + prochaines tâches               |

Soit ~8-9 h/semaine, suffisant pour terminer cette roadmap en 9 mois si tu gardes le scope strict.

Le livrable GitHub attendu à la fin

Avec :

* un README par projet,

* une image/animation du résultat,

* les commandes d’exécution,

* les métriques de base.

Ça montre non seulement que tu connais les concepts, mais surtout que tu sais construire, tester, mesurer et documenter un système autonome.

# Projet reinforcement : robot humanoïde

Repo pour le projet de reinforcement learning. 

## Installation des librairies 

Toutes les librairies nécessaires et les versions dans le fichiers **requirements.txt**, pour les installer exécuter la ligne de code suivante : 

```
pip install -r requirements.txt
```


Y a deux fichiers : 
- **bipedal_walker_2d.py**
- **humanoid_walker_3d.py**

Comme les noms l'indiquent, l'un permet d'entrainer le modèle pour le robot bipède en 2D avec un processus d'optimisation ARS et l'autre le robot humanoïde en 3D avec un processus PPOT. 

Pour exécuter les scripts, il faut simplement exécuter les lignes suivantes :

```shell
conda create --name name_of_your_env python=3.9
conda activate name_of_your_env
pip install -r requirements.txt
python bipedal_walker_2d.py
```

Ou alors

```shell
conda create --name name_of_your_env python=3.9
conda activate name_of_your_env
pip install -r requirements.txt
python humanoid_walker_3d.py
```

Les résultats seront alors stockés dans un sous dossier 'results/2D' ou 'results/3D'




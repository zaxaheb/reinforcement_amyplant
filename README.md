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
Puis 

```
python bipedal_walker_2d.py
```

Ou alors

```
python humanoid_walker_3d.py
```

Les résultats seront alors stockés dans un sous dossier 'results/2D' ou 'results/3D'

Si au moment d'éxécuter le script 3d, cette erreur s'affiche : 

```
pyvirtualdisplay.abstractdisplay.XStartError: No success after 10 retries. Last stderr: b"_XSERVTransmkdir: ERROR: euid != 0,directory /tmp/.X11-unix will not be created.\n_XSERVTransSocketUNIXCreateListener: mkdir(/tmp/.X11-unix) failed, errno = 2\n_XSERVTransMakeAllCOTSServerListeners: failed to create listener for local\n(EE) \nFatal server error:\n(EE) Cannot establish any listening sockets - Make sure an X server isn't already running(EE) \n"
```

Il faut exécuter ces cellules

```
mkdir /tmp/.X11-unix
sudo chmod 1777 /tmp/.X11-unix
sudo chown root /tmp/.X11-unix/
```



### Ressources

PPOT :
- https://datascientest.com/proximal-policy-optimization-tout-savoir
- https://openai.com/research/openai-baselines-ppo
- https://towardsdatascience.com/proximal-policy-optimization-ppo-explained-abed1952457b

ARS :
- https://towardsdatascience.com/introduction-to-augmented-random-search-d8d7b55309bd
- https://github.com/melih-unsal/augmented-random-search
 
Reinforcement learning :
- https://datascientest.com/reinforcement-learning
- https://towardsdatascience.com/reinforcement-learning-101-e24b50e1d292
- https://datascientest.com/reinforcement-learning-comment-apprendre-a-une-ia-a-jouer-au-snake

Refs :
- https://colab.research.google.com/github/shariq101/Teaching-a-Bipedal-walker-using-ARS/blob/master/BipedalWalker_V_2.ipynb
- https://www.codeproject.com/script/Content/ViewReadingList.aspx?rlid=27

    




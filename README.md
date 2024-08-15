# Installation de pip

## Commandes d'installation

## Documentation et explications

Ce guide explique comment installer pip, le gestionnaire de paquets pour Python, en utilisant la méthode du script bootstrap.

### Prérequis

- Python 3 installé sur votre système
- Accès à Internet
- Droits d'administrateur (pour certains systèmes)

### Explications détaillées des commandes

#### Première commande : Téléchargement du script

Cette commande utilise `curl` pour télécharger le script d'installation de pip. Voici le détail :

- `curl` est un outil en ligne de commande pour transférer des données avec URL.
- `https://bootstrap.pypa.io/get-pip.py` est l'URL du script d'installation de pip.
- `-o get-pip.py` indique à `curl` de sauvegarder le fichier téléchargé sous le nom `get-pip.py` dans le répertoire courant.

#### Deuxième commande : Exécution du script

Cette commande exécute le script téléchargé pour installer pip. Voici ce qui se passe :

1. `python3` lance l'interpréteur Python 3.
2. `get-pip.py` est le script que Python va exécuter.
3. Le script effectue les actions suivantes :
   - Vérifie la version de Python installée.
   - Télécharge la dernière version de pip compatible avec votre système.
   - Installe pip et ses dépendances.
   - Configure pip pour qu'il soit accessible en ligne de commande.

### Vérification de l'installation

Après l'installation, vérifiez que pip est correctement installé en exécutant :
Cette commande devrait afficher la version de pip installée sur votre système.

### Remarques importantes

- Sur certains systèmes, vous devrez peut-être utiliser `sudo python3 get-pip.py` pour avoir les droits nécessaires à l'installation.
- Il est recommandé de toujours utiliser la dernière version de pip. Vous pouvez mettre à jour pip avec la commande :
  ### Pourquoi utiliser cette méthode ?

1. Universalité : Cette méthode fonctionne sur la plupart des systèmes d'exploitation.
2. Mise à jour : Elle installe toujours la dernière version stable de pip.
3. Fiabilité : Le script provient de la source officielle (Python Packaging Authority).

### Alternatives

- Sur certains systèmes Linux, pip peut être installé via le gestionnaire de paquets (par exemple, `apt-get install python3-pip` sur Debian/Ubuntu).
- Sur Windows, pip est généralement inclus avec les installations récentes de Python depuis python.org.

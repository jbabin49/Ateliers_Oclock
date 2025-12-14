<h1 align=center>Fonctionnement d'un OS</h1>

# Procédure de démarrage

1. on appuie sur le bouton "power" d'allumage
2. le BIOS initialise tous les composants de la carte mère et certains périphérique
3. le BIOS identifie les périphériques internes et externes
4. le BIOS démarre le système d'exploitation
5. une fois le système d'exploitation démarré, on peut lancer nos applications !

En anglais, on dit qu'un ordinateur "boot" pour indiquer qu'il démarre. Ce terme est souvent utilisé en Français également.

Redémarrer un ordi = reboot !

# Processus

Un processus (process, en anglais) est un programme en cours d'exécution sur un ordinateur.

L'exécution d'un processus dure un certain temps, avec un début et parfois une fin. Un processus peut être démarré par l'utilisateur ou par un autre processus.

Les applications que nous utilisons tous les jours, sont souvent composées d'un ensemble de processus.

## Système multitâches

Un système d'exploitation est multitâches s'il permet d'exécuter, de façon apparemment simultanée, plusieurs programmes.

Un coeur de processeur ne peut exécuter qu'une seule tâche à la fois, pour pouvoir lancer plusieurs programmes simultanément, le système d'exploitation va passer de l'exécution d'un processus à un autre très rapidement.

# Pilotes

## Pilote de périphérique

Un pilote (driver, en anglais) est un programme qui permet au système d'exploitation (et aux autres logiciels) d'interagir avec un périphérique connecté à l'ordinateur.

Chaque périphérique a son propre pilote. Sans pilote, le périphérique ne peut pas être utilisé !

## Composants internes

Les composants matériels internes à l'ordinateur, comme la carte graphique, peuvent également nécessiter un pilote.

## Pilotes génériques

Les systèmes d'exploitation proposent leurs propres pilotes génériques censés fonctionner avec la plupart des périphériques. 

Ils proposent en général moins de fonctionnalités que les pilotes fournis par le constructeur du périphérique.

## Plug-and-play

Certains périphériques sont dits "plug-and-play", pour sous-entendre qu'il suffit de les connecter et qu'ils sont directement utilisables.

En réalité, ces périphériques utilisent eux-aussi des pilotes, c'est juste que le système d'exploitation détermine automatiquement le pilote à utiliser sans nécessiter d'action de l'utilisateur.

## Installation de pilotes

Si le système d'exploitation ne propose pas de pilote générique pour notre périphérique, pas le choix, il faudra l'installer nous-même !

Les pilotes sont en général téléchargeables depuis le site officiel du fabricant du périphérique.

<h3 align=center>⚠️</h3>
<p align=center>Attention, certains sites spécialisés, non-officiels, proposent le téléchargement de milliers de pilotes.<br>
Évitez au maximum ces sites et passez par le site du fabricant, pour éviter de télécharger un virus.<br>
Les pilotes doivent être conçus pour le système d'exploitation installé sur votre ordinateur (un pilote Windows ne fonctionnera pas sous MacOS !)</p> 

# Fichiers

Un fichier est une **collection d'informations** portant un nom, enregistré sur un média tel qu'un disque dur, une bande magnétique, un disque optique ou une mémoire fiash.

Le système d'exploitation s'occupe de créer, modifier et détruire les fichiers et les répertoires (dossiers).

Le système d'exploitation permet également de modifier les **attributs** des fichiers : leur _nom_, _date de création/modification_, _type de contenu_, _taille_ et _emplacement_.

Il permet également de gérer des permissions : des autorisations qui indiquent si un utilisateur spécifique peut lire, écrire (modifier) ou exécuter le fichier.

# Installer un OS

## Système d'exploitation pré-installé

Quand on achète un ordinateur ou un smartphone, celui-ci est en général fourni avec un système d'exploitation pré-installé.

Mais il est tout à fait possible d'installer nous-même ce système !

### Pour quoi faire ?

Plein de raisons possibles :

* installer un système différent de celui fourni
* installer une nouvelle version du système (pour passer à Windows 11, par exemple)
* ré-installer le système pour résoudre un bug, ou en cas de présence d'un virus
* ré-installer le système pour le configurer différemment

En entreprise, on ré-installe en général systématiquement un système d'exploitation sur les ordinateurs neufs.

## Les différents supports

### CD/DVD d'installation

Pour installer un système d'exploitation, on a besoin d'un média d'installation.

Pendant de nombreuses années, les systèmes d'exploitation étaient installés à partir d'un DVD ou d'un CD-ROM fourni par l'éditeur.

De nos jours, avec la disparition des lecteurs de disques optiques, on utilise plutôt une clé USB.

### Image ISO

La clé USB d'installation n'est en général pas fournie par l'éditeur du système d'exploitation !

Nous allons devoir la créer nous-même depuis un autre ordinateur, avec un utilitaire prévu à cet effet et en utilisant une image disque (aussi appelé image ISO).

Une image disque est une copie conforme (une "photo") du contenu d'un disque optique ou magnétique. Il existe différent formats d'images disque, mais le format ISO est le plus utilisé.

## Booter sur le média d'installation

Pour installer un système d'exploitation sur un ordinateur, il va falloir faire en sorte que l'ordinateur démarre un système d'exploitation "léger" stocké sur le média d'installation (que ce soit une clé USB ou 
un DVD).

Il faudra potentiellement pour cela modifier l'ordre de démarrage dans le BIOS de l'ordinateur.

Ce système léger va nous permettre d'effectuer l'installation, en nous posant différentes questions.

Une fois le nouveau système installé, il suffit de redémarrer l'ordinateur et de retirer le média d'installation (ou modifier à nouveau l'ordre de démarrage dans le BIOS), pour que l'ordinateur démarre sur le nouveau système installé sur l'un des disques durs.

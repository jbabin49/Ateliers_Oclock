<h1 align=center>BIOS, UEFI, MBR et GPT</h1>

Comprenez les technologies fondamentales du démarrage informatique et du partitionnement des disques.

---

# Introduction au BIOS

## La Puce BIOS

La puce BIOS est un **composant matériel essentiel** de la carte mère. Cette puce est généralement de petite taille et soudée directement sur la carte mère.

Le BIOS stocké dans cette puce est un **logiciel de bas niveau**, qui contrôle des fonctions critiques comme :
- L'initialisation de la mémoire
- L'initialisation du processeur
- L'initialisation des périphériques

Elle stocke le **firmware BIOS**, qui initialise le matériel lors de la mise sous tension de l'ordinateur et permet de démarrer le système d'exploitation.

**Rôle principal** : Assurer la communication entre les composants matériels et le système d'exploitation.

## Le Clear CMOS

Le **Clear CMOS** est un processus permettant de réinitialiser les paramètres du BIOS ou de l'UEFI à leurs valeurs par défaut d'usine.

Le **CMOS** (Complementary Metal-Oxide-Semiconductor) est une petite mémoire sur la carte mère qui stocke les paramètres de configuration du BIOS, comme :
- L'ordre de démarrage
- La date et heure
- Les paramètres de CPU

**Quand c'est nécessaire** : En cas de mauvaise configuration, d'overclocking incorrect ou de problèmes de démarrage.

**Comment faire** : Il se fait en retirant brièvement la pile CMOS ou en utilisant un jumper Clear CMOS sur la carte mère.

---

# Concept de Firmware

## Qu'est-ce que le Firmware ?

Le **firmware** est un logiciel intégré directement dans le matériel d'un appareil. Il se situe entre le matériel (hardware) et le système d'exploitation, permettant aux composants de fonctionner ensemble.

Les firmwares sont présents dans une large gamme d'appareils :
- Ordinateurs
- Smartphones
- Routeurs
- Imprimantes

Ils sont **essentiels** pour le bon fonctionnement de ces dispositifs, car ils contrôlent les fonctions matérielles de base.

**Exemples courants** :
- BIOS
- UEFI
- Firmware de cartes graphiques
- Microcontrôleurs dans les appareils électroniques

## BIOS et UEFI comme Firmwares

Le BIOS et l'UEFI sont des exemples de **firmwares** qui gèrent l'initialisation du système et le démarrage de l'OS.

Le firmware peut être **mis à jour** pour :
- Corriger des bugs
- Améliorer la sécurité
- Ajouter de nouvelles fonctionnalités

**Important** : Les mises à jour doivent être effectuées avec **précaution**.

---

# Le BIOS (Basic Input/Output System)

## Présentation

Le **BIOS** est un firmware qui assure l'initialisation matérielle et le chargement du système d'exploitation lors du démarrage. Il est souvent utilisé sur les systèmes plus anciens.

Le BIOS initialise les composants matériels comme :
- La mémoire
- Le processeur
- Les périphériques

Puis il recherche le **secteur de démarrage** sur le disque pour lancer le système d'exploitation.

## Utilisation et Accès

L'utilisation du BIOS est basique, mais sa navigation est **compliquée**, car elle se fait uniquement au clavier et les menus sont souvent datés.

**Caractéristiques** :
- Chaque BIOS a ses propres réglages et son propre fonctionnement
- L'accès au BIOS varie selon les constructeurs
- En général, les touches **F2** ou **DEL** permettent d'y accéder

## Paramètres Majeurs du BIOS

Le BIOS permet de configurer des éléments clés du système :
- **Boot Order** : Définit l'ordre dans lequel les périphériques sont vérifiés pour démarrer (disque dur, clé USB, etc.)
- **Legacy USB** : Permet l'utilisation de périphériques USB pendant le démarrage
- **Heure et date** : Réglage du système
- **S.M.A.R.T Monitoring** : Surveillance de l'état des disques
- **Processeur** : Configuration et gestion de l'alimentation (Wake-on-LAN)

### Fonctionnalités Avancées du BIOS

Le BIOS est responsable de :
- La gestion de la mémoire RAM
- Le contrôle des ventilateurs et des températures
- La surveillance des composants critiques du système
- Les options de sécurité (mots de passe pour protéger l'accès)

Il permet également de :
- Activer la **virtualisation matérielle** (Intel VT-x ou AMD AMD-V)
- Configurer les ressources systèmes comme les interruptions (IRQ) et les accès directs à la mémoire (DMA)
- Être **mis à jour (flashé)** pour prendre en charge de nouvelles fonctionnalités ou corriger des erreurs

## Mettre à Jour le BIOS (Flasher)

Mettre à jour le firmware de sa carte mère permet de rendre son système **plus stable et plus performant**.

**Attention** : La mise à jour du BIOS ou de l'UEFI n'est **pas une démarche sans risques**. Il y a un risque (certes faible) que la mise à jour plante et si c'est le cas... la carte mère serait H.S. ! 💥

## Limitations du BIOS

Le BIOS présente plusieurs limitations :
- Ne peut pas gérer des disques de plus de 2 To
- Fonctionne en **mode 16 bits**, ce qui limite ses performances et sa flexibilité
- Simple à configurer et compatible avec des systèmes anciens
- Limité en termes de capacités de disque et de gestion de ressources
- Pas de USB 3.0 ou de Secure Boot natif

---

# L'UEFI (Unified Extensible Firmware Interface)

## Présentation

L'**UEFI** est le successeur du BIOS, conçu pour offrir plus de **flexibilité** et de **fonctionnalités modernes**.

Contrairement au BIOS, l'UEFI propose :
- Une interface plus **intuitive** avec la prise en charge de la souris
- Des menus plus **graphiques**
- Des fonctionnalités plus **avancées**

Il peut **gérer des disques de plus de 2 To** grâce à l'utilisation de la table de partitionnement **GPT (GUID Partition Table)**.

## Paramètres Majeurs de l'UEFI

L'UEFI offre des paramètres avancés comme :
- **Secure Boot** : Empêche le démarrage de systèmes d'exploitation non signés
- **CSM** (Compatibility Support Module) : Imite le BIOS pour assurer la compatibilité avec des anciens systèmes
- **Fast Boot** : Réduit le temps de démarrage en éliminant certaines étapes non essentielles
- **Network Boot (PXE)** : Permet de démarrer un système depuis un réseau
- **TPM** (Trusted Platform Module) : Options de sécurité avancées pour le chiffrement des données

## Secure Boot

Le **Secure Boot** est une fonctionnalité de sécurité intégrée dans l'UEFI qui garantit que **seul un système d'exploitation signé et approuvé** peut démarrer sur un ordinateur.

Il empêche le chargement de logiciels malveillants au démarrage, comme :
- Rootkits
- Autres programmes non autorisés

### Fonctionnement

Lors du démarrage, le Secure Boot vérifie que le chargeur de démarrage du système d'exploitation possède une **signature numérique valide**. Si la signature est approuvée, le processus de démarrage se poursuit. Sinon, l'ordinateur refusera de démarrer le système, protégeant ainsi contre les menaces.

Cette fonctionnalité peut être **activée ou désactivée** dans les paramètres de l'UEFI, selon les besoins de l'utilisateur.

## Fast Boot

Le **Fast Boot** est une fonctionnalité de l'UEFI qui accélère le processus de démarrage en réduisant ou en sautant certaines étapes d'initialisation matérielle non essentielles.

Cette option est conçue pour **améliorer les temps de démarrage**, notamment sur les ordinateurs modernes.

Lorsque le Fast Boot est activé, l'UEFI passe rapidement certaines vérifications matérielles, comme :
- Tests de mémoire RAM
- Détection exhaustive des périphériques

Cela permet de démarrer le système d'exploitation **beaucoup plus rapidement**.

## Comparaison BIOS vs UEFI

Le BIOS et l'UEFI diffèrent sur plusieurs points importants :

| Aspect | BIOS | UEFI |
|--------|------|------|
| **Mode** | 16 bits | 32 ou 64 bits |
| **Taille disque** | Limité à 2 To | Plus de 2 To |
| **Interface** | Textuelle et simple | Graphique et intuitive |
| **Fonctionnalités** | Basiques | Avancées (Secure Boot, etc.) |
| **Gestion disques** | MBR | GPT |

---

# Partitionnement des Disques

## MBR (Master Boot Record)

Le **Master Boot Record (MBR)** est un ancien système de partitionnement qui gère l'organisation et le démarrage des disques durs.

**Localisation** : Il est situé dans le tout premier secteur du disque et contient les informations nécessaires pour démarrer le système d'exploitation.

### Structure du MBR

Le MBR divise un disque en **4 partitions principales au maximum**. Si plus de partitions sont nécessaires, une des partitions principales doit être une **partition étendue**, qui peut contenir plusieurs partitions logiques.

Le MBR est utilisé **principalement sur les anciens systèmes**.

### Limitations du MBR

Le MBR présente plusieurs limitations :
- Limite le nombre de partitions à **4 principales**
- Ne supporte que des disques d'une taille **maximale de 2 To**
- **Vulnérable à la corruption** car toutes les informations de démarrage sont stockées dans un seul secteur

**Note** : La limitation de taille du disque est la même que le BIOS !

## Le GPT (GUID Partition Table)

Le **GPT** est un système de partitionnement moderne conçu pour **remplacer le MBR**. Il utilise des **ID uniques** pour chaque partition et supporte jusqu'à **128 partitions par disque**.

### Avantages du GPT

Le GPT supporte :
- **Disques de plus de 2 To**
- **Meilleure protection** contre la corruption des données grâce à un mécanisme de **CRC32**
- **Fonctionnement optimal** avec l'UEFI, permettant une plus grande flexibilité et sécurité

## Comparaison MBR vs GPT

| Aspect | MBR | GPT |
|--------|-----|-----|
| **Partitions** | 4 principales | Jusqu'à 128 |
| **Taille disque** | 2 To max | Grande capacité |
| **Protection** | Basique | CRC32 |
| **Compatibilité** | Anciens systèmes | Systèmes modernes |
| **Firmware** | BIOS | UEFI |

---

# Systèmes de Fichiers

## Introduction

Les **systèmes de fichiers** sont des structures qui organisent et gèrent la manière dont les données sont stockées et récupérées sur des disques.

Trois des systèmes de fichiers les plus utilisés sont :
- NTFS
- FAT32
- exFAT

Chaque système de fichiers a ses propres caractéristiques, avantages et limitations, et est utilisé dans différents contextes selon les besoins en matière de compatibilité, de performances, et de sécurité.

## NTFS (New Technology File System)

Le **NTFS** est un système de fichiers développé par **Microsoft** pour les systèmes Windows.

Il est le **système par défaut** pour les disques durs modernes utilisés sur Windows.

### Caractéristiques du NTFS

- **Supporte des fichiers de grande taille** (plus de 4 Go) et des volumes jusqu'à 16 To et plus
- Offre des fonctionnalités avancées :
  - Chiffrement des fichiers
  - Compression
  - Permissions de sécurité détaillées
- **Utilise un journal de fichiers** pour protéger contre la corruption des données en cas de panne

**Inconvénient** : Compatibilité limitée avec les systèmes autres que Windows

## FAT32 (File Allocation Table 32)

Le **FAT32** est un système de fichiers plus ancien et largement compatible. Il est couramment utilisé sur des périphériques de stockage comme les clés USB et les cartes mémoire.

### Caractéristiques du FAT32

- **Compatible** avec la majorité des systèmes d'exploitation :
  - Windows
  - macOS
  - Linux
  - Plupart des appareils électroniques
- **Limité à des fichiers de 4 Go maximum** et à des volumes de 32 Go pour Windows

**Inconvénients** :
- Ne supporte pas les grands fichiers (> 4 Go)
- Offre moins de sécurité et de fonctionnalités avancées que NTFS

## exFAT (Extended File Allocation Table)

Le **exFAT** est un système de fichiers créé pour combler l'écart entre FAT32 et NTFS, particulièrement pour les supports de stockage amovibles comme les clés USB et les disques externes.

### Caractéristiques de exFAT

- **Supporte des fichiers de très grande taille** (au-delà de 4 Go) sans les limitations de FAT32
- **Compatible** avec Windows, macOS, et de nombreux appareils
- Plus léger que NTFS

**Avantages** :
- Support des grands fichiers
- Bonne compatibilité entre systèmes

**Inconvénients** :
- Moins de fonctionnalités avancées par rapport à NTFS (chiffrement, permissions)

## Comparaison des Systèmes de Fichiers

| Système | Taille Max Fichier | Taille Max Volume | Compatibilité | Fonctionnalités |
|---------|-------------------|------------------|---------------|-----------------|
| **NTFS** | > 4 Go | Jusqu'à 16 To+ | Windows (principalement) | Sécurité, compression, journalisation |
| **FAT32** | 4 Go | 32 Go (Windows) | Windows, macOS, Linux, appareils | Simplicité, large compatibilité |
| **exFAT** | > 4 Go | 128 Po (théorique) | Windows, macOS, appareils | Légèreté, compatibilité grands fichiers |

## Choisir le Bon Système de Fichiers

Le choix du système de fichiers dépend de plusieurs facteurs :

**NTFS** :
- Idéal pour les disques durs internes dans un environnement Windows
- Où la sécurité et la gestion de grands fichiers sont essentielles

**FAT32** :
- Recommandé pour les clés USB ou les cartes mémoire destinées à être utilisées sur une variété d'appareils
- Limité à de petits fichiers

**exFAT** :
- Meilleur choix pour les périphériques amovibles nécessitant la compatibilité multi-plateformes
- Avec des fichiers de grande taille

---

# Conclusion

Maîtriser le **BIOS**, l'**UEFI**, le **MBR** et le **GPT** est essentiel pour comprendre le démarrage informatique et gérer efficacement les disques durs modernes. Ces technologies fondamentales permettent aux ordinateurs de fonctionner et d'organiser les données de manière fiable et performante. 🖥️⚙️

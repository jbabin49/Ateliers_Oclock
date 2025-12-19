<h1 align=center>Incidents Hardware et Réglementation</h1>

Maîtrisez le diagnostic des pannes matérielles et les obligations légales en matière de recyclage et protection des données.

---

# Objectifs et Introduction

## Objectifs de la Journée

Cette formation couvre trois aspects essentiels :
- Diagnostic et résolution de pannes matérielles
- Réglementation DEEE (Déchets d'Équipements Électriques et Électroniques)
- Réglementation RGPD (Règlement Général sur la Protection des Données)

**Bonus** : Mini-quizz sous forme de jeux pendant la journée !

## Introduction au Dépannage (Focus Matériel)

Points importants à retenir :
- Vous ne serez **pas experts** à l'issue de cette introduction (il faut des années de pratique)
- Vous aurez une idée de **comment diagnostiquer une panne**
- Vous aurez la capacité d'**échanger plus facilement** avec un professionnel

---

# Anatomie et Diagnostic de Base

## Analogie : L'Ordinateur comme un Corps Humain

Pour mieux comprendre le fonctionnement d'un ordinateur :
- Le **système sanguin** permet de faire circuler l'énergie
- Le **système nerveux** permet de faire circuler la data (les informations) entre le cerveau et les organes

## Avant de Démonter un Ordinateur

Avant d'en arriver à une phase de diagnostic plus poussée, effectuez quelques opérations simples :
- Effectuer un **nettoyage de poussière** dans l'ordinateur (souvent responsable)
- **Débrancher tous les périphériques** (garder clavier/souris + écran seulement)
- **Tester avec des câbles** de branchement en bon état de fonctionnement (on y pense pas souvent)
- Faire un **test de démarrage** pour analyser le problème et avoir un premier diagnostic

## Composants Clés

### La Pile du BIOS/UEFI

Ne pas oublier la petite pile qui permet d'alimenter le BIOS quand le PC est éteint !

---

# Diagnostic des Écrans Noirs

## Si j'ai un Écran Noir, de Quoi Ça Peut Venir ?

Voici les différentes sources à vérifier :
- Le **branchement des prises** (écran, PC)
- **Changer les câbles électriques** (extérieurs)
- **Changer l'alimentation** de l'ordinateur
- **Débrancher la carte graphique** (utiliser la sortie de la carte mère)
- **Vérifier le branchement de la RAM**
- **Vérifier la pile du BIOS** (la changer si besoin)
- **Tenter un clear CMOS** (jump sur carte mère)

## Les Autres Causes d'un Écran Noir

Dans certains cas plus grave :
- **Changer la carte mère** par une autre (attention à la compatibilité processeur et RAM)
- **Changer le processeur**

## Écran Noir avec Message d'Erreur

Souvent, le **disque dur** en est la principale cause.

---

# Diagnostic des Erreurs de Démarrage

## Erreur Windows au Démarrage

En cas d'échec lors de la dernière extinction, essayez de démarrer le PC dans les différents modes de Windows :
- Mode normal
- Mode sans échec

## Machine qui s'Allume avec Autres Erreurs

Il s'agit probablement d'un **problème logiciel** :
- **Virus**
- **Problème de démarrage** dû à une mauvaise mise à jour
- **Autres divers problèmes**

## Résumé (Partie 1) : Identification des Symptômes

En première étape, on identifie les symptômes :
- Écran noir ?
- Écran comportant des erreurs ?
- Poussière accumulée ?
- Comportement anormal de l'ordinateur
- Sons inhabituels
- Analyse des messages d'erreurs du BIOS/UEFI

## Résumé (Partie 2) : Recherche des Causes

En deuxième étape, on recherche des causes possibles (pour cela, on isole le problème) :
- Est-ce qu'un composant est en panne et empêche le démarrage ? (carte mère, processeur, RAM, alimentation électrique)
- On utilise des outils de diagnostics intégrés une fois qu'on a au moins accès à un écran BIOS

---

# Outils de Diagnostic et Monitoring

## Introduction aux Outils

Ici, nous allons voir quelques outils de diagnostic/monitoring sur le matériel (dont beaucoup gratuits). Cela permettra d'analyser les faiblesses en détail !

**Important** : Cette étape doit être faite uniquement si le PC démarre !

## Le Multimètre

Utiliser un **multimètre** peut permettre de vérifier correctement l'alimentation électrique.

## Le BIOS/UEFI

**POST (Power-On Self Test)** : Comprendre les résultats du POST pour détecter les composants en panne avant le démarrage du système d'exploitation.

## Le Test du Processeur

Le logiciel `CPU-Z` est la référence en la matière. Des sondes permettent de voir les températures/fréquences des composants.

## Le Test de la Carte Graphique

Le logiciel `GPU-Z` est la référence en la matière. Des sondes permettent de voir les températures/fréquences des composants.

## La RAM Uniquement

Les logiciels `MemTest64`, `MemTest86` ou `MemTest86+` (bootable) permettent de vérifier si la RAM va bien !

## Le Stockage (Disque Mécanique/SSD)

Le logiciel `CrystalDiskMark` permet de faire des tests de performance de votre disque.

**Attention** : l'état de santé n'y figure pas (on utilisera `SSD Life` ou `HWMonitor` dans ce cas). Il existe également d'autres outils (comme `chkdsk` en CMD).

## Les Ventilateurs, Vitesses, etc.

Le logiciel `HWMonitor` permet d'avoir ce genre de statistiques (très complet).

## L'Alimentation

Le logiciel `OCCT` est très complet. **Attention** : il fera souffler les équipements pendant les tests !

## Les Batteries

Le logiciel `BatteryBar` est gratuit et permet de faire des tests. Ce test est à réaliser sur 1 à 2 semaines.

---

# Tests Approfondis des Composants

## Alimentation (PSU)

- **Vérification des tensions** : Utilisation d'un multimètre pour mesurer les différentes tensions de sortie (3.3V, 5V, 12V) sur les différents connecteurs
- **Test de charge** : Utilisation d'une alimentation de test pour vérifier la stabilité de l'alimentation sous charge
- **Détection de surchauffe** : Utilisation d'un thermomètre infrarouge pour détecter la surchauffe

## Mémoire RAM

- **Test avec MemTest86+** : Outils de diagnostic de la mémoire pour détecter des erreurs sur chaque barrette de RAM
- **Test manuel** : Enlever une barrette de RAM à la fois pour voir si l'ordinateur fonctionne correctement avec une seule barrette

## Disques Durs

- **Utilisation de CrystalDiskInfo** : Connaître l'état de santé du disque
- **Test de surface du disque** : Utilisation d'outils comme HD Tune pour vérifier la surface des disques et identifier les secteurs défectueux
- **Vérification des câbles SATA** : Rebrancher ou remplacer les câbles pour éliminer un problème de connexion

## Carte Mère et Processeur

- **POST et codes d'erreurs** : Utilisation des bips ou des codes d'erreurs générés par la carte mère pour identifier des pannes liées au processeur ou à la carte mère
- **Test avec une carte mère de remplacement** : Si disponible, tester le processeur sur une autre carte mère pour éliminer l'hypothèse d'une panne de carte mère

## Carte Graphique

- **Test dans un autre ordinateur** : Installer la carte graphique sur un autre ordinateur pour vérifier si le problème persiste
- **Test avec une autre carte graphique** : Si possible, utiliser une autre carte graphique pour voir si le problème disparaît
- **Problèmes de pilotes** : Vérifier si les pilotes de la carte graphique sont à jour ou mal configurés

---

# Réparation/Remplacement de Matériel

## Réparation des Composants

**RAM défectueuse** :
- En fonction de l'erreur, il peut être possible de simplement nettoyer les contacts des barrettes ou de les repositionner correctement dans les slots

**Disque dur / SSD défectueux** :
- Réparation via la réallocation des secteurs défectueux (dans la mesure du possible) ou formatage bas niveau
- Si le disque est critique pour les données, envisager un clonage avant d'effectuer des réparations

**Réparation du BIOS/UEFI** :
- Si la carte mère ou le BIOS est corrompu, un reset du BIOS ou une mise à jour du firmware peut parfois résoudre le problème

## Remplacement des Composants

**Mémoire RAM** :
- Si la barrette est défectueuse, remplacer par un modèle compatible

**Alimentation (PSU)** :
- Si le test des tensions ou des câbles révèle des problèmes, remplacer l'alimentation par une nouvelle
- Veiller à choisir une puissance adaptée aux composants du système

**Carte graphique ou carte mère** :
- Si le problème est identifié comme étant lié à l'un de ces composants, remplacement obligatoire si aucune réparation n'est possible
- Veiller à la compatibilité avec le reste du système

## Autres Cas Complexes

Certains problèmes sont plus difficiles à diagnostiquer car ils ne se produisent pas de manière constante ou surviennent après une modification du système :
- Pannes intermittentes
- Surchauffe
- Conflits matériels

---

# Réglementation DEEE

## Présentation de la Réglementation DEEE

Les DEEE (Déchets d'Équipements Électriques et Électroniques) sont des équipements électriques et électroniques en fin de vie, qui nécessitent un traitement spécifique pour réduire leur impact environnemental.

**Origine de la réglementation** : La directive européenne 2012/19/UE sur les DEEE

**Qu'est-ce que les DEEE** : Tout équipement fonctionnant à l'électricité ou utilisant des piles est considéré comme un DEEE une fois en fin de vie

## Les Enjeux

Les équipements électroniques contiennent des matériaux polluants (plomb, mercure, cadmium) qui peuvent être **dangereux** pour la santé et l'environnement s'ils ne sont pas traités correctement.

## Les Impacts

- **Pollution des sols et des eaux** en cas de mise en décharge non contrôlée
- **Consommation de ressources rares** comme les métaux précieux (or, cuivre)
- **Augmentation des déchets électroniques** à l'échelle mondiale, avec un volume estimé à 50 millions de tonnes par an

## Les Obligations Légales

En tant que technicien, il est essentiel de comprendre comment la réglementation DEEE s'applique dans le cadre professionnel, notamment lors du remplacement ou de la mise au rebut d'équipements informatiques.

### Rôles et Responsabilités

**Pour les producteurs et distributeurs** :
- Obligation de prendre en charge la collecte et le recyclage des DEEE vendus aux clients
- Obligation de financer le traitement des équipements mis sur le marché après 2005

**Pour les entreprises et les professionnels** :
- Obligation de trier les DEEE et de les confier à une filière agréée pour le recyclage
- Suivi des DEEE
- **Destruction des données** (sensibles) notamment sur les supports de stockage

## Les Sanctions

- **Amendes et sanctions administratives** si les entreprises ne respectent pas leurs obligations de gestion des DEEE
- **Environnement** : conséquences graves pour l'image de l'entreprise en cas de pollution causée par une mauvaise gestion des déchets électroniques

## Processus de Collecte et de Traitement des DEEE

- Tri et collecte des équipements
- Stockage temporaire sécurisé
- Transport vers des filières agréées
- Traitement et recyclage
- Destruction des données

## Les Bonnes Pratiques

**Réduire la quantité de DEEE** :
- Privilégier le reconditionnement et la réutilisation du matériel

**Autres bonnes pratiques** :
- Sensibiliser au recyclage
- Suivi et traçabilité des déchets
- Utiliser des logiciels de destruction des données (`DBAN`, `Eraser` par exemple)

---

# Réglementation RGPD

## Introduction au RGPD

- **Adopté en** mai 2018
- **Objectif** : Renforcer la protection des données personnelles dans l'UE
- **Champ d'application** : Toute organisation traitant des données personnelles de citoyens de l'UE
- **Sanctions** : Jusqu'à 20 millions d'euros ou 4 % du CA annuel mondial

## La CNIL (Commission Nationale de l'Informatique et des Libertés)

**Rôle** : Autorité administrative indépendante française chargée de veiller à la protection des données personnelles

**Création** : Fondée en 1978, renforcée par le RGPD en 2018

**Missions principales** :
1. Informer les individus et les professionnels
2. Veiller à l'application de la législation
3. Contrôler et sanctionner les entreprises en cas de non-conformité

**Exemple** : Audits réguliers des pratiques des entreprises en matière de traitement de données

## Principes Clés du RGPD

1. **Légalité, loyauté, transparence**
2. **Limitation des finalités**
3. **Minimisation des données**
4. **Exactitude des données**
5. **Limitation de la conservation**
6. **Intégrité et confidentialité**
7. **Responsabilité (Accountability)**

## Droits des Individus

1. **Droit d'accès**
2. **Droit de rectification**
3. **Droit à l'effacement** ("droit à l'oubli")
4. **Droit à la limitation du traitement**
5. **Droit à la portabilité des données**
6. **Droit d'opposition**
7. **Droit de ne pas faire l'objet** de décisions automatisées

## Mise en Œuvre du RGPD en Entreprise

### Analyse d'Impact sur la Protection des Données (AIPD)

- **Obligatoire** si risque élevé pour les droits et libertés des personnes
- **Méthodologie** : Identifier les risques, évaluer l'impact, proposer des mesures

### Registre des Activités de Traitement

- **Obligatoire** pour toutes les entreprises traitant des données personnelles
- Doit recenser les traitements effectués : objectifs, nature des données, durée de conservation

### Consentement des Personnes

- **Consentement libre, spécifique, éclairé et univoque**
- **Exemple** : Consentement pour les cookies sur les sites web

## Mesures de Sécurité Techniques et Organisationnelles

- **Pseudonymisation et chiffrement** des données
- **Gestion des accès** : mots de passe sécurisés, gestion des utilisateurs
- **Sauvegardes et audits réguliers**
- **Formation des employés** à la protection des données

## Le Délégué à la Protection des Données (DPO)

**Rôle** : Conseiller, superviser la conformité, point de contact avec la CNIL

**Obligation** : DPO obligatoire pour les organismes publics et grandes entreprises

**Responsabilités** : Veiller à la conformité RGPD, former les équipes

## En Cas de Violation des Données

**Définition** : Perte, vol, divulgation non autorisée des données personnelles

**Obligations** :
- **Notifier la CNIL** dans les 72h
- **Informer les personnes concernées** si risque élevé

**Exemples** : Fuite de données par email, disque dur non chiffré perdu

## Plan de Réponse aux Incidents

- **Prévention** : Mise en place d'un plan de réponse pour limiter les dommages
- **Importance** : Limiter les risques en cas de violation de données

## Outils et Ressources

- **Outils logiciels** pour la gestion de la conformité RGPD : gestion des consentements, chiffrement, sécurité des données
- **Ressources en ligne** : Guides de la CNIL pour accompagner les entreprises

---

# Conclusion

## Points Clés à Retenir

**1. Diagnostic et Résolution de Pannes Matérielles** :
- Approche méthodique
- Utilisation des outils de diagnostic
- Importance de la maintenance proactive

**2. Réglementation DEEE** :
- Respect des obligations de recyclage
- Gestion des déchets électroniques dans le cadre légal

**3. Conformité RGPD** :
- Protection des données personnelles
- Mise en place de mesures techniques et organisationnelles
- Droits des individus et obligations des entreprises

## Message Final

**Importance de la vigilance** : Respecter les bonnes pratiques de diagnostic et de conformité pour éviter les pannes matérielles et les sanctions légales

**Rôle de la formation continue** : La technologie et la réglementation évoluent constamment, d'où l'importance de rester à jour ! 🔧⚖️

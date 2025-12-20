<h1 align=center>Pratiques ITIL & GLPI</h1>

Description à compléter.

---

Pratiques ITIL & GLPI
1
Introduction à GLPI
GLPI (Gestion Libre de Parc Informatique) est une solution open-
source de gestion des services informatiques. Il permet la gestion
des actifs informatiques, des tickets d'incidents, des demandes de
service et des processus d'assistance, le tout basé sur les bonnes
pratiques de l'ITIL.
GLPI propose des interfaces intuitives pour administrer un parc
informatique, gérer les incidents, et offrir une meilleure visibilité des
processus IT.
2
Concepts ITIL appliqués à
GLPI
L'ITIL (Information Technology Infrastructure Library) est un
ensemble de bonnes pratiques pour la gestion des services IT. Dans
GLPI, ces pratiques se retrouvent dans la gestion des incidents, des
demandes de service, et la gestion des changements.
3
Les principaux processus ITIL dans GLPI :
Gestion des incidents : Traitement des interruptions de service.
Gestion des demandes : Réponses aux demandes utilisateurs.
Gestion des changements : Suivi des modifications dans l’infrastructure IT.
4
Interface de gestion des
actifs
L'interface de gestion des actifs dans GLPI permet de recenser et
gérer tous les équipements informatiques de l'entreprise
(ordinateurs, serveurs, imprimantes, etc.).
Fonctionnalités principales :
Ajout, modification et suppression des actifs.
Suivi de l'historique d'utilisation.
Liaison des actifs avec des tickets ou des contrats de maintenance.
5
Interface de gestion des
utilisateurs
GLPI permet de gérer les utilisateurs et leurs rôles dans le système.
Chaque utilisateur peut avoir un rôle spécifique, par exemple :
administrateur, technicien, ou utilisateur final.
L'interface permet de :
Créer des comptes utilisateurs.
Assigner des groupes et profils (droits d'accès).
Suivre l'historique des actions des utilisateurs.
6
Liste des profils GLPI
7
Hotliner
Le Hotliner est responsable de la résolution des problèmes
techniques des utilisateurs.
Il répond aux appels et fournit une assistance de premier niveau.
8
Technicien
Le Technicien s'occupe des incidents plus complexes.
Il gère le suivi des demandes de support et la gestion des
équipements.
9
Administrateur
L'Administrateur dispose d'un accès complet à toutes les
fonctionnalités de GLPI.
Il gère la configuration du système, les utilisateurs et les profils, ainsi
que la génération de rapports.
10
Self-Service
Le profil Self-Service permet aux utilisateurs d'accéder à une
interface pour :
Soumettre des demandes de support
Suivre l'état de leurs tickets
Accéder à des ressources utiles
Il favorise l'autonomie des utilisateurs et réduit la charge de travail
du support.
11
Observer
Le Observer est destiné aux managers ou responsables.
Il permet de surveiller les statistiques, analyser les rapports et les
activités du support.
Il aide à prendre des décisions pour améliorer les processus.
12
Interface de gestion des
tickets
L'interface de gestion des tickets est centrale dans GLPI. Elle permet
de créer, suivre et résoudre les incidents et demandes de service.
Fonctionnalités :
Création de tickets via une interface utilisateur intuitive.
Suivi de l'évolution des tickets avec un workflow de traitement.
Priorisation des tickets en fonction de l'impact et de l'urgence.
13
Indicateurs de Ticket
14
Indicateurs de performance
Dans GLPI, vous pouvez suivre plusieurs indicateurs de ticketing
pour évaluer la performance de votre équipe de support.
Ces indicateurs incluent :
Le temps moyen de résolution des tickets
Le nombre total de tickets ouverts
La satisfaction globale des utilisateurs
Ces données permettent de prendre des décisions éclairées pour
améliorer la qualité du support technique.
15
TTO (Temps Total
d'Ouverture)
Le TTO mesure le temps écoulé entre la création du ticket et sa prise
en charge par un technicien.
Il est utilisé pour suivre la rapidité de réaction du support après la
déclaration d’un incident ou d’une demande.
Ticket créé à 10h00
Technicien commence à le traiter à 10h30
👉 TTO = 30 minutes
16
TTR (Temps Total de
Résolution)
Le TTR mesure le temps total entre la création du ticket et sa
résolution (ou clôture).
Cet indicateur est clé pour évaluer l'efficacité du processus de
résolution.
Ticket créé à 10h00
Ticket résolu à 12h00
👉 TTR = 2 heures
17
TTO Interne & TTR Interne
Le TTO Interne mesure la durée pendant laquelle un ticket est ouvert au sein de
l'équipe de support, en excluant les temps d'attente externes.
Le TTR Interne mesure le temps de résolution interne, en excluant les délais
externes.
En optimisant ces indicateurs, vous pouvez améliorer l'efficacité de
l'équipe et offrir une meilleure expérience utilisateur.
18
Base de connaissances
(Knowledge Base)
GLPI propose une base de connaissances intégrée, permettant de
documenter les solutions aux problèmes récurrents ou les
procédures standard.
Elle offre :
Un accès rapide à des articles techniques pour les techniciens et les utilisateurs.
La possibilité de lier des articles à des tickets pour faciliter la résolution des
incidents.
19
Workflow de gestion des
incidents (ITIL)
Selon ITIL, un incident est toute interruption ou réduction de la
qualité de service.
Dans GLPI, le processus de gestion des incidents suit ces étapes :
Détection et enregistrement de l'incident via un ticket.
Classification et priorisation selon les critères d'impact et d'urgence.
Résolution de l'incident par les techniciens assignés.
Clôture du ticket une fois la solution validée.
20
Interface de gestion des
demandes
La gestion des demandes de service dans GLPI permet de traiter les
requêtes utilisateurs, telles que l'installation de logiciels ou l'accès à
de nouvelles ressources.
L'interface propose :
La création de demandes spécifiques à chaque service.
Un suivi des demandes avec des étapes de validation.
La possibilité d'associer des actifs ou des utilisateurs à chaque demande.
21
Gestion des contrats et
équipements
GLPI permet de gérer les contrats liés aux équipements IT, comme
les contrats de maintenance ou de garantie.
L'interface de gestion des contrats inclut :
Le suivi des dates de début et de fin des contrats.
L'ajout de prestataires et la gestion de la facturation.
Des alertes pour anticiper la fin d'un contrat.
22
Ordinateur portable HP
Contrat : Garantie constructeur
Fournisseur : HP
Expiration : 15/06/2023
23
Imprimante multifonction Canon
Contrat : Contrat de maintenance
Fournisseur : Canon
Expiration : 31/12/2024
24
Serveur Dell
Contrat : Contrat de support 24/7
Fournisseur : Dell
Expiration : 01/09/2025
25
Suivi des stocks
L'interface de gestion des stocks dans GLPI permet de suivre le
matériel informatique disponible, de sa commande à sa livraison.
Fonctionnalités :
Gestion des fournisseurs et commandes.
Suivi des quantités de matériel et des consommables.
Association des stocks aux tickets ou projets.
26
Suivi des licences
GLPI offre une interface dédiée à la gestion des licences logicielles,
permettant de s'assurer que l'organisation reste en conformité avec
ses obligations.
Fonctionnalités :
Suivi des licences et de leur durée.
Association des licences avec des actifs.
Alertes pour les licences expirantes.
27
Gestion des changements
(ITIL)
Dans l'ITIL, la gestion des changements consiste à contrôler et gérer
toute modification dans l'infrastructure IT. GLPI permet d'enregistrer
et de suivre les changements à travers des tickets dédiés.
Fonctionnalités :
Création de tickets de changement.
Suivi du processus d'approbation et de validation.
Liaison avec des incidents ou projets.
28
Interface de gestion des
projets
GLPI permet la gestion des projets IT, de la planification à l'exécution.
Chaque projet peut être suivi dans l'interface dédiée, avec la
possibilité de créer des sous-tâches et d'affecter des ressources.
Fonctionnalités :
Création de projets et gestion des échéances.
Suivi des ressources (personnel, matériel).
Liaison des projets avec des tickets ou changements.
29
Rapports et statistiques
L'interface de rapports dans GLPI permet de générer des statistiques
sur l'ensemble des actifs, des tickets et des utilisateurs.
Fonctionnalités :
Rapports détaillés sur les tickets : résolution, durée, incidents récurrents.
Suivi des performances des techniciens et des équipes.
Statistiques sur l'utilisation des actifs et des ressources.
30
Notifications et alertes
GLPI inclut un système de notifications pour tenir les utilisateurs
informés de l'avancement de leurs tickets, projets ou demandes.
Fonctionnalités :
Notifications par email ou directement dans l'interface.
Alertes pour les tickets en attente, les contrats expirants, ou les changements à
approuver.
Paramétrage personnalisé des notifications pour chaque utilisateur.
31
Intégration avec d'autres
outils
GLPI peut être intégré avec d'autres outils IT, tels que :
Des solutions de supervision réseau (comme Nagios).
Des outils de gestion des identités pour la synchronisation des utilisateurs.
Des solutions de backup et de monitoring.
Ces intégrations permettent d'automatiser certaines tâches et
d'offrir une vue globale sur l'infrastructure IT.
32
Gestion des droits et
sécurité
GLPI propose une gestion fine des droits d'accès et des profils
utilisateurs pour sécuriser les données sensibles.
Fonctionnalités :
Définition de profils utilisateurs avec des niveaux de permissions variés.
Restriction de l'accès à certaines interfaces ou données selon le rôle de l'utilisateur.
Journalisation des actions pour garantir la traçabilité des modifications.
33
Personnalisation des
interfaces
L'interface de GLPI peut être personnalisée pour répondre aux
besoins spécifiques de chaque organisation.
Fonctionnalités :
Modification des champs dans les tickets, les actifs, ou les projets.
Création de formulaires personnalisés pour les demandes ou les incidents.
Intégration de plugins pour étendre les fonctionnalités.
34
Plugins et extensions
GLPI dispose d'un écosystème riche de plugins qui permettent
d'ajouter des fonctionnalités supplémentaires, telles que :
La gestion de téléphones mobiles (MDM).
Des modules de facturation.
Des intégrations avec des outils de virtualisation ou de cloud.
35
Conclusion
GLPI est une solution complète pour la gestion des services IT, en
intégrant des concepts issus de l'ITIL pour la gestion des incidents,
des demandes et des changements.
Ses interfaces intuitives, couplées à ses nombreuses fonctionnalités,
en font un outil indispensable pour les équipes IT cherchant à
améliorer l'efficacité de leur service et la gestion de leurs actifs.
36
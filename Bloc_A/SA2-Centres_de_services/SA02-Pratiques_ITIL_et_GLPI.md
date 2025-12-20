
<h1 align=center>Pratiques ITIL & GLPI</h1>

Présentation des concepts ITIL appliqués à la gestion des services informatiques avec GLPI.

---

# Introduction à GLPI

GLPI (Gestion Libre de Parc Informatique) est une solution open-source de gestion des services informatiques.

- Gestion des actifs informatiques, tickets d'incidents, demandes de service et processus d'assistance
- Interfaces intuitives pour administrer un parc informatique, gérer les incidents et améliorer la visibilité des processus IT

---

# Concepts ITIL appliqués à GLPI

L'ITIL (Information Technology Infrastructure Library) est un ensemble de bonnes pratiques pour la gestion des services IT.

- Gestion des incidents : traitement des interruptions de service
- Gestion des demandes : réponses aux demandes utilisateurs
- Gestion des changements : suivi des modifications dans l’infrastructure IT

---

# Interface de gestion des actifs

Permet de recenser et gérer tous les équipements informatiques de l'entreprise (ordinateurs, serveurs, imprimantes, etc.).

**Fonctionnalités principales :**
- Ajout, modification et suppression des actifs
- Suivi de l'historique d'utilisation
- Liaison des actifs avec des tickets ou des contrats de maintenance

---

# Interface de gestion des utilisateurs

Permet de gérer les utilisateurs et leurs rôles dans le système.

- Création de comptes utilisateurs
- Assignation de groupes et profils (droits d'accès)
- Suivi de l'historique des actions des utilisateurs

## Profils GLPI

- **Hotliner** : Résolution des problèmes techniques, assistance de premier niveau
- **Technicien** : Gestion des incidents complexes, suivi des demandes de support
- **Administrateur** : Accès complet, gestion du système, utilisateurs, profils et rapports
- **Self-Service** : Soumission de demandes, suivi des tickets, accès à des ressources utiles
- **Observer** : Suivi des statistiques, analyse des rapports, aide à la décision

---

# Interface de gestion des tickets

Permet de créer, suivre et résoudre les incidents et demandes de service.

**Fonctionnalités :**
- Création de tickets via une interface intuitive
- Suivi de l'évolution des tickets avec workflow
- Priorisation selon l'impact et l'urgence

## Indicateurs de ticket et de performance

- Temps moyen de résolution des tickets
- Nombre total de tickets ouverts
- Satisfaction globale des utilisateurs

**TTO (Temps Total d'Ouverture) :**
Temps entre la création du ticket et sa prise en charge par un technicien

**TTR (Temps Total de Résolution) :**
Temps entre la création du ticket et sa résolution (ou clôture)

**TTO/TTR Interne :**
Durée de traitement interne, hors délais externes

---

# Base de connaissances (Knowledge Base)

Permet de documenter les solutions aux problèmes récurrents ou procédures standard.

- Accès rapide à des articles techniques
- Lien possible entre articles et tickets

---

# Workflow de gestion des incidents (ITIL)

1. Détection et enregistrement de l'incident via un ticket
2. Classification et priorisation (impact/urgence)
3. Résolution par les techniciens assignés
4. Clôture du ticket après validation

---

# Interface de gestion des demandes

Permet de traiter les requêtes utilisateurs (installation de logiciels, accès à de nouvelles ressources, etc.).

- Création de demandes spécifiques à chaque service
- Suivi des demandes avec étapes de validation
- Association d'actifs ou d'utilisateurs à chaque demande

---

# Gestion des contrats et équipements

Permet de gérer les contrats liés aux équipements IT (maintenance, garantie, etc.).

- Suivi des dates de début et de fin
- Ajout de prestataires, gestion de la facturation
- Alertes pour anticiper la fin d'un contrat

**Exemples :**
| Équipement                  | Contrat                | Fournisseur | Expiration    |
|-----------------------------|------------------------|-------------|--------------|
| Ordinateur portable HP      | Garantie constructeur  | HP          | 15/06/2023   |
| Imprimante multifonction Canon | Contrat de maintenance | Canon       | 31/12/2024   |
| Serveur Dell                | Support 24/7           | Dell        | 01/09/2025   |

---

# Suivi des stocks

Permet de suivre le matériel informatique disponible, de la commande à la livraison.

- Gestion des fournisseurs et commandes
- Suivi des quantités et consommables
- Association des stocks aux tickets ou projets

---

# Suivi des licences

Permet de gérer les licences logicielles et la conformité.

- Suivi des licences et de leur durée
- Association des licences avec des actifs
- Alertes pour licences expirantes

---

# Gestion des changements (ITIL)

Contrôle et gestion des modifications dans l'infrastructure IT via des tickets dédiés.

- Création de tickets de changement
- Suivi du processus d'approbation et de validation
- Liaison avec incidents ou projets

---

# Interface de gestion des projets

Permet la gestion des projets IT, de la planification à l'exécution.

- Création de projets et gestion des échéances
- Suivi des ressources (personnel, matériel)
- Liaison des projets avec tickets ou changements

---

# Rapports et statistiques

Génération de statistiques sur les actifs, tickets et utilisateurs.

- Rapports détaillés sur la résolution, durée, incidents récurrents
- Suivi des performances des techniciens et équipes
- Statistiques sur l'utilisation des actifs et ressources

---

# Notifications et alertes

Système de notifications pour informer les utilisateurs de l'avancement de leurs tickets, projets ou demandes.

- Notifications par email ou dans l'interface
- Alertes pour tickets en attente, contrats expirants, changements à approuver
- Paramétrage personnalisé des notifications

---

# Intégration avec d'autres outils

GLPI peut être intégré avec d'autres outils IT :
- Supervision réseau (Nagios)
- Gestion des identités (synchronisation utilisateurs)
- Solutions de backup et monitoring

---

# Gestion des droits et sécurité

Gestion fine des droits d'accès et profils utilisateurs pour sécuriser les données sensibles.

- Définition de profils utilisateurs avec permissions variées
- Restriction d'accès selon le rôle
- Journalisation des actions pour la traçabilité

---

# Personnalisation des interfaces

L'interface de GLPI peut être adaptée aux besoins de chaque organisation.

- Modification des champs dans tickets, actifs, projets
- Création de formulaires personnalisés
- Intégration de plugins pour étendre les fonctionnalités

---

# Plugins et extensions

GLPI dispose d'un écosystème riche de plugins pour ajouter des fonctionnalités :
- Gestion de téléphones mobiles (MDM)
- Modules de facturation
- Intégrations avec outils de virtualisation ou cloud

---

# Conclusion

GLPI est une solution complète pour la gestion des services IT, intégrant les concepts ITIL pour la gestion des incidents, demandes et changements. Ses interfaces intuitives et ses nombreuses fonctionnalités en font un outil indispensable pour les équipes IT souhaitant améliorer l'efficacité du service et la gestion des actifs.
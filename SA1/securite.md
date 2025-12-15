<h1 align=center>Sécurité informatique</h1>
<h3 align=center>Introduction / Bonnes pratiques</h3>

# Pourquoi ?

## _Il y a des métiers spécialisés dans la sécurité informatique : pourquoi devrions-nous nous en soucier ?_

* la sécurité est l'affaire de tous
* toutes les entreprises n'ont pas les moyens d'embaucher un/des expert(s)
* en freelance/indépendant, on est seul ! (et on doit s'en occuper, ou sous-traiter)

## REAC

Et surtout : c'est au programme de votre Titre Pro.

Vous devez :

* connaître les bonnes pratiques de sécurité
* pouvoir sensibiliser les utilisateurs à ces bonnes pratiques
* respecter la charte / les règles de sécurité de l'entreprise
* prendre en compte la sécurité lors de vos interventions
* connaître les acteurs de la sécurité informatique

(liste non-exhaustive)

## Intéret de la sécurtié informatique

Dans notre société hyper-connectée, de nombreux aspects de notre vie dépendent du bon fonctionnement de nos infrastructures informatiques.

On passe par un ordinateur pour :

* déclarer nos revenus & payer nos impôts
* prendre rdv chez le médecin et faire des télé-consultations
* faire nos courses ou commander à manger
* stocker nos photos de famille
* communiquer avec nos proches
* etc...

On comprend bien que la sécurité de ces systèmes informatiques est primordiale, personne ne souhaite voir ses données divulguées aux yeux de tous (et ce, même si on a “rien à cacher”).

Pire, les conséquences d’une attaque informatique peuvent parfois être bien plus graves qu’une fuite de données ...

Vous avez entendu parler de [Stuxnet](https://fr.wikipedia.org/wiki/Stuxnet) ?

# 5 indicateurs/critères

Quand on parle de la sécurité d'un système informatique et des données qui y transitent, on vise plusieurs objectifs, on mesure la sécurité du système selon certains indicateurs/critères.

## Intégrité

Garantir l'intégrité d'une donnée, c'est garantir qu'elle n'ait pas pu être altérée, modifiée à l'insu du système.

## Confidentialité

Seules les personnes qui y ont été autorisées, qui sont légitimes à y avoir accès, doivent pouvoir accéder à une donnée spécifique.

## Authentification / authenticité

Le système informatique doit être capable d'identifier avec certitude un utilisateur.

On identifie un utilisateur via un identifiant unique (adresse email, nom d'utilisateur), puis on authentifie/certifie cette identité au moyen d'un facteur d'authentification (mot de passe, empreinte digitale, etc).

## Disponibilité

Un système disponible est un système fonctionnel, accessible, utilisable.

On doit maintenir le bon fonctionnement du système informatique, le maintenir en conditions opérationnelles.

## Non-répudiation / Traçabilité / Preuve

La non-répudiation (aussi appelée l'imputation), est le fait d'empêcher qu'un utilisateur puisse nier avoir effectué une transaction.

Cela se matérialise par la conservation de preuves, par la tracabilité de toutes les transactions.

# Métiers de la sécu info

Il existe de nombreux métiers dans le domaine de la sécurité informatique.

L'ANSSI a essayé d'en faire la [liste](https://cyber.gouv.fr/offre-de-service/formations-entrainement-et-decouverte-des-metiers/observatoires-des-metiers/observatoire-des-metiers-enquete-2020/).

La liste suivante et loin d'être exhaustive !

## Cryptologue

C’est un mathématicien spécialisé dans la cryptologie.

Il fait un travail de recherche, c’est lui qui va concevoir et analyser les algorithmes et protocoles cryptographiques qu'on va utiliser/mettre en place dans nos systèmes informatique par la suite.

## DSSI / RSSI

_Directeur / Responsable de la Sécurité des Systèmes d'Information_

C'est le responsable de la sécurité du SI dans une entreprise.

⚠️ Il est recommandé que ce ne soit pas la même personne que le DSI.

## Auditeur / Pentester

C'est un expert technique qui va réaliser des audits de sécurité, aussi appelés tests d'intrusion (penetration test en anglais, d'où le terme pentest).

Son but ? Identifier les vulnérabilités/failles présentes dans le système (avant qu'un hacker les trouve).

## DPO

_Data Protection Officer_

C'est la personne chargée du respect du RGPD dans une entreprise.

Pas nécessairement informaticien, il sera mobilisé en cas de fuite de données personnelles.

## Expert sécurité

Un administrateur système/réseau expert/spécialisé en sécurité.

ou

Un développeur expert/spécialisé en sécurité.

ou

...

## Consultant / formateur

Chaque secteur en possède son lot : des consultants proposants diverses prestations de conseil/d'accompagnement, des formateurs qui vendent des formations plus ou moins pertinentes, etc...

# Grands principes

Des trucs qui peuvent sembler évidents, mais à garder en tête quand on parle de cybersécurité.

## Menace #1

La plus grande menace est, et sera toujours ... l'utilisateur.

Qu'il soit mal-intentionné ou simplement distrait/maladroit, dans tous les cas : on ne peut pas lui faire confiance.

## Privilège minimum

Le principe du privilège minimum doit être appliqué partout : 

chaque groupe, service, utilisateur doit avoir uniquement accès à ce qui lui est strictement indispensable pour remplir à bien ses missions.

## Defense in Depth

Le principe de “Defense in Depth” (défense en profondeur) doit être appliqué : la sécurité doit être organisée en plusieurs niveaux indépendants, en plusieurs couches. Si un niveau est compromis, le niveau suivant devra bloquer l’attaque.

## Être parano : c'est bien

Nous devons être (un peu) paranoïaques, suspicieux : si quelque chose semble suspect, ou semble trop beau pour être vrai, c’est sûrement le cas (ce principe permet notamment de se protéger du social engineering).

## Sécurité absolue ?

La sécurité absolue (parfaite, inviolable) n’existe pas.

On doit faire un compromis : notre mission va être d’essayer de sécuriser au maximum nos systèmes tout en s’assurant qu’ils restent fonctionnels, utilisables.

Il y aura toujours de nouvelles failles de sécurité, il faut donc se préparer à l’échec des mesures de sécurité que nous aurons mises en place : créez des PRA/PCA (Plan de Reprise/Continuité d’Activité), faites des sauvegardes (on en reparlera) !

## Le plus faible des composants

La sécurité d’un système est égale à la sécurité du plus faible de ses composants.

Inutile d’avoir une porte blindée si la porte de derrière ne ferme pas bien !

## Secure by design

On doit penser à la sécurité dès la phase de conception, de stratégie. 

Ce principe s’oppose au fait de ne penser à la sécurité qu'à la fin d'un projet informatique, il faut au contraire prendre en compte la sécurité dès le début du projet.

Certaines décisions (le choix d'une technologie, d'un logiciel, d'un protocole, etc.), prises souvent très tôt dans un projet, peuvent impacter la sécurité de tout le SI. 

Une fois le projet bien avancé, revenir sur ces choix peut impliquer devoir tout refaire.

## Loi de murphy

Cette loi (satirique) bien connue dit que “tout ce qui est susceptible d’aller mal ira mal”, ou que “s'il y a plusieurs façons de faire quelque chose, et que l'une d'elles conduit à un désastre, alors il y aura quelqu'un pour le faire de cette façon”.

En sécurité (informatique, mais pas que) cette loi doit être érigée comme un grand principe. 

Non, le pire n’est pas toujours certain, mais par prudence, il faut concevoir notre application comme si cette loi était vraie.

# Acteurs
... du monde de la sécurité informatique !

## ANSSI

L’Agence Nationale de la Sécurité des Systèmes d’Information (ANSSI) est un service gouvernemental Français.

Ce service, créé en 2009, est rattaché au Secrétariat Général de la Défense et de la Sécurité Nationale (SGDSN) et sa mission première est d’assister le Premier ministre dans l’exercice de ses responsabilités en matière de défense et de sécurité nationale.

L’ANSSI n’assiste pas que le Premier ministre : elle a un rôle d’autorité nationale en matière de sécurité des systèmes d’information.

L’agence publie des recommandations, des livres-blancs, s’assure de la sécurité des OIV (Opérateurs d’Importance Vitale), gère le CERT-FR (voir ci-après).

## CSIRT / CERT

Les CSIRT (Computer Security Incident Response Team) et CERT (Computer Emergency Response Team) sont des équipes d’experts en sécurité informatique chargées de réagir en cas d’incident informatique.

Le terme CERT est le plus utilisé, mais c’est une marque déposée qui appartient à l’université américaine Carnegie Mellon. Les CSIRT peuvent demander à utiliser cette marque.

En France, l’ANSSI opère un CSIRT qui s’appelle CERT-FR (anciennement CERTA). 

Son rôle est de prévenir les attaques en effectuant une veille sur les nouvelles failles découvertes, faire de la prévention auprès des entreprises, être un relais et centraliser la communication (avec le réseau mondial des CERT par exemple).

à retenir : Le CERT-FR publie notamment des alertes de sécurité, la liste est accessible sur son site [cert.ssi.gouv.fr](https://www.cert.ssi.gouv.fr/).

## CVE / MITRE

MITRE est une organisation à but non-lucratif américaine. Cette organisation publie le dictionnaire CVE (Common Vulnerabilities and Exposures).

Une CVE est une vulnérabilité, une faille, qui peut être exploitée par des hackers et causer plus ou moins de dégâts sur un système d’information. La criticité potentielle d’une vulnérabilité est évaluée à l’aide du CVSS (Common Vulnerability Scoring System).

L’identifiant CVE est une référence de la forme CVE-YYYY-NNNN (ou YYYY est l’année de publication et NNNN un identifiant). Pour chaque CVE, MITRE publie une description succincte de la vulnérabilité ainsi que des informations supplémentaires permettant d’en savoir plus ou de s’en prémunir.

Le dictionnaire des CVE est accessible [ici](https://www.cve.org/).

## CNIL

La CNIL (Commission Nationale Informatique & Libertés) est une autorité administrative indépendante française. 

La CNIL est chargée de veiller à ce que l’informatique soit au service du citoyen et qu’elle ne porte atteinte ni à l’identité humaine, ni aux droits de l’homme, ni à la vie privée, ni aux libertés individuelles ou publiques.

à retenir : Son rôle est (entre autres) de veiller au respect du RGPD et au respect de la loi Informatique et Libertés, et de prononcer des sanctions (jusqu’à 20 millions d’€) à l’égard d’organismes qui ne respectent pas ces lois ou règlements.

En cas d’intrusion dans notre système (et que certaines données personnelles ont pu être compromises), on doit obligatoirement notifier la CNIL et les personnes concernées.

## OWASP

OWASP (Open Web Application Security Project) est une organisation à but non lucratif spécialisée sur la sécurité des applications web.

OWASP publie des recommandations pour la sécurisation des applications web et propose aussi différents outils (pédagogiques ou techniques) liés à la sécurité sur le web.

Ses projets les plus connus :

* Top10 : la liste des dix risques de sécurité les plus critiques ou les plus fréquemment rencontrés sur le web
* ZAP (Zed Attack Proxy) : outil de scan de failles de sécurité web
* WSTG (Web Security Testing Guide) : un guide très complet à destination du pentester
* Cheat Sheet Series : plein de mémos sur la sécurité des apps web
* ASVS (Application Security Verification Standard) : un PDF très complet, pour aller plus loin

# Et nous ? (notre mission)

La sécurité informatique s’appréhende sous trois aspects complémentaires : la prévention, la détection et la réaction.

En tant que technicien informatique, on peut intervenir sur ces trois aspects.

## Prévention

* anticiper / identifier les risques
* sensibiliser les utilisateurs
* limiter l'impact d'attaques éventuelles
* tester les politiques de sécurité/sauvegarde
* respecter les bonnes pratiques
* faire de la veille
* etc...

## Détection

* surveiller le réseau, le parc (monitoring, analyse de logs)
* réagir en cas d'alerte automatisée

## Réaction

* suivre le PCA/PRA pour rétablir et/ou maintenir le système en conditions opérationnelle
* restaurer des sauvegardes
* prévenir / communiquer (CNIL, assurances, dépôt de plainte, etc.)

# Mots de passe

## Mots de passe : bonnes pratiques

Un mot de passe sécurisé est un mot de passe généré aléatoirement, d’une longueur suffisante, et unique à un système (il ne faut surtout pas utiliser le même mot de passe partout).

Un mot de passe ne doit pas contenir d’informations personnelles (nom d’un animal de compagnie, date de naissance/mariage, etc.), ne doit pas être uniquement composé de substitutions de caractères (exemple : b0bm4rl3y) ou de mots présents dans la langue anglaise/française, et il faut bien entendu éviter [les mots de passe les plus souvent utilisés](https://en.wikipedia.org/wiki/List_of_the_most_common_passwords).

## Gestionnaire de mots de passe

Retenir un mot de passe unique pour chaque site, généré aléatoirement, est impossible.

Seule solution ? Stocker nos mots de passe quelque-part. 

Mieux que le carnet papier, mieux que de les stocker dans votre navigateur web, il faut utiliser un gestionnaire de mot de passe, qui stocke ces mots de passe de façon chiffrée.

## Facteurs d'authentification

Il existe différents types de facteurs d'authentification :

* facteur de connaissance :
  * mot de passe
  * code pin
* facteur de possession :
  * clef
  * carte à puce / carte magnétique
  * code reçu par SMS (possession du téléphone)
  * code OTP/TOTP (possession de la "graine")
* facteur biologique :
  * empreinte digitale
  * reconnaissance rétinienne / vocale

On parle parfois aussi de "facteur réactionnel", un geste qu'on peut reproduire, comme une signature.

## 2FA / MFA

2FA = two-factor auth. / MFA = multi-factor auth.

Dès que possible, il faut activer/mettre en place l'authentification à facteurs multiples (deux minimum).

Le principe ? Après avoir saisi un mot de passe (facteur de connaissance), on nous demande un code reçu par SMS (facteur de possession).

# Antivirus / Antimalware

On parle de sécurité, ce serait dommage de ne pas parler des logiciels antivirus !

[Qu'est ce qu'un logiciel antivirus ?](https://fr.wikipedia.org/wiki/Logiciel_antivirus)

## À retenir

Deux grands modes de fonctionnement :

* analyse de la signature (hash) des fichiers
* analyse du comportement des programmes (méthode heuristique)

Types de malwares
La liste ci-dessous est non-exhaustive, et certains malwares

peuvent être dans plusieurs "catégories".

* ransomware : chiffre les données, exige une rançon (souvent en bitcoins) pour obtenir la clé de déchiffrement
* spyware : espionne l'activité de l'utilisateur, permet de voler des données ou des comptes
* adware : virus publicitaire, sert à générer de l'argent via des clics sur les pubs affichées
* cheval de troie : code malicieux embarqué dans une application qui semble légitime
* ver : virus capable de s'auto-répliquer, de contaminer d'autres machines via le réseau (ou d'autres moyens)
* rootkit : malware furtif, conçu pour ne pas pouvoir être détecté, ou en tout cas très dif�cilement*
* keylogger : type de spyware, qui enregistre toutes les frappes au clavier. Peut aussi être matériel !
* coinminer : malware qui mine du bitcoin (ou autres crypto-monnaies) à l'insu de l'utilisateur
* botnet : réseau de machines "zombies", contaminées par un malware, permettant de faire par exemple des attaques DDoS

# Cryptographie

Quelques petites notions !

## Chiffrement vs. hachage









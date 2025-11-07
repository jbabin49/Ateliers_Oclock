# Challenge Packet Tracer SA3 - Réseaux

## Contexte

Une nouvelle entreprise vous recrute pour professionnaliser son réseau. Actuellement, les salariés sont connectés en WiFi sur des box FAI avec du matériel hétérogène.

Le parc informatique va être complètement renouvelé.

L'entreprise est en pleine expansion, et recrute fréquemment de nouveaux salariés. Actuellement, il y a 59 collaborateurs, vous y compris, mais l'entreprise pourrait dépasser 200 salariés ou plus dans les mois/années à venir ! 📈

Voici les différents services de l'entreprise ainsi que le nombre de salariés par service :

 - commerciaux : 16
 - communication : 5
 - comptabilité : 5
 - direction : 4
 - ressources humaines : 2
 - juridique : 2
 - recherche et développement : 23
 - informatique : 2

L'entreprise a des bureaux à Paris et à Lille, mais ils envisagent à terme d'ouvrir un site par département Français.

À Paris, on retrouve la direction, la comptabilité, le service juridique, la communication et les ressources humaines. Il y a également 10 commerciaux, 12 ingénieurs R&D et un informaticien.

Le site de Lille compte 11 ingénieurs R&D, 6 commerciaux et un informaticien.

Sur le site de Paris, une salle serveur va être créée et équipée 4 serveurs. Le coeur du réseau y sera installé. Les salariés du service R&D sont dans un batiment différent, équipé d'une petite baie informatique, de quoi y installer un peu de matériel réseau ! La baie du batiment R&D sera relié à la salle serveur avec une fibre optique.

Les salariés peuvent travailler de façon nomade : depuis leur domicile en télétravail ou en déplacement chez des clients pour les commerciaux, par exemple. Ils se connectent via un VPN sur le routeur du site de Paris au réseau de l'entreprise (plus d'infos ci-dessous).

### Étape 1 - Plan d'adressage

Voici les sous-réseaux minimum à créer :

 * Paris :
   * LAN (tous les PC fixes et portables)
   * DMZ (zone démilitarisée, pour les serveurs, voir ci-dessous)
   * WiFi public (pour les visiteurs, filaire obligatoire pour les salariés)

 * Lille :
   * LAN (tous les PC fixes et portables)
   * WiFi public (pour les visiteurs, filaire obligatoire pour les salariés)

 * VPN (un sous-réseau dans lequel se trouvent les machines des collaborateurs à distance)

#### Plan

Je prends large sur les LAN pour prévenir l'expansion de l'entreprise.

* Paris

<center>
  
|Nom|Équipements|Adresse réseau|Adresses dispos|Passerelle|
|---|-----------|--------------|---------------|----------|
|P-LAN|41|192.168.1.0/24|254|192.168.1.1|
|P-WifiPublic|?|192.168.2.0/24|254|192.168.2.1|
|P-Serveurs|4|192.168.3.0/28|14|192.168.3.1|

</center>

* Lille

<center>
  
|Nom|Équipements|Adresse réseau|Adresses dispos|Passerelle|
|---|-----------|--------------|---------------|----------|
|L-LAN|18|10.0.0.0/24|254|10.0.0.1|
|L-WifiPublic|?|10.0.1.0/24|254|10.0.1.1|

</center>

* VPN

<center>
  
|Nom|Équipements|Adresse réseau|Adresses dispos|Passerelle|
|---|-----------|--------------|---------------|----------|
|VPN|59|172.16.0.0/24|254|172.16.0.1|

</center>

# PACTOLS
<p>Le thésaurus PACTOLS produit par la Fédération et Ressources sur l'Antiquité (<a href="http://www.frantiq.fr" target="_blank">Frantiq</a>, Groupement de services du CNRS) est mis à disposition selon les termes de la licence <a href="https://spdx.org/licenses/ODbL-1.0.html#" target="_blank">ODC Open Database License (ODbL) v1.0</a></p><p>Fondé(e) sur une œuvre consultable librement ici: <a href="http://pactols.frantiq.fr" target="_blank">http://pactols.frantiq.fr</a>.</p><p>Les autorisations au-delà du champ de cette licence peuvent être obtenues à <a href="http://www.frantiq.fr" target="_blank">http://www.frantiq.fr</a>.</p>

<b>Un thésaurus pour l'archéologie</b>

PACTOLS est l’unique vocabulaire français pour l’archéologie qui soit libre, multilingue (FR, en, de, it, es, nl, ar),normalisé (SKOS) et interopérable (ISO 25964).

Son organisation en dossiers thématiques lui a donné son nom : Peuples et cultures, Anthroponymes, Chronologie (depuis la préhistoire jusqu’à l’époque contemporaine), Toponymes, Oeuvres, Lieux, Sujets. Ces derniers couvrent tous les sujets intéressant l'archéologie et les sciences de l'Antiquité.

Elaboré à partir de la littérature scientifique recensée au <a href="http://catalogue.frantiq.fr" target="_blank">Catalogue collectif indexé</a> des bibliothèques du réseau Frantiq et des lexiques spécialisés, il est mis à jour avec l'aide des experts des domaines scientifiques et suit l'évolution de la discipline.

Il constitue un réservoir de métadonnées spécialisées appliquées aujourd’hui à toutes les pratiques de la discipline : enregistrement de terrain, bases de données de travail et bibliographiques, édition scientifique, valorisation du patrimoine archéologique, etc.
# PACTOLS via le Webservices REST de <a href="https://github.com/miledrousset/opentheso" target="_blank">Opentheso</a> 

Recherche par Identifiant (Ark) avec précision du format :

https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy.rdf

https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy.json

https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy.jsonld

https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy.ttl


Recherche par l’identifiant du concept avec précision du format :
https://pactols.frantiq.fr/opentheso/api/TH_1.13175.rdf
uri REST = https://pactols.frantiq.fr/opentheso/api/
id du thesaurus = TH_1
id du concept =  13175
format = rdf
formats valides : (.rdf), (.json), (.jsonld), (.ttl).


Recherche avec Curl en choisissant le header :
curl -L --header "Accept: application/rdf+xml" https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy
curl -L --header "Accept: application/json" https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy
curl -L --header "Accept: application/ld+json" https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy
curl -L --header "Accept: text/turtle" https://pactols.frantiq.fr/opentheso/api/26678/pcrtkOgxvd4Ijy

valable aussi pour la recherche par l’identifiant du concept.


Recherche par valeur :
curl -L --header "Accept: application/rdf+xml" https://pactols.frantiq.fr/opentheso/api/search?q=amphore&lang=fr&theso=TH_1


Toutes ces commandes sont possibles pour le header
curl -L --header "Accept: application/rdf+xml »
curl -L --header "Accept: text/turtle » 
curl -L --header "Accept: application/json »
curl -L --header "Accept: application/ld+json »

curl -L --header "Accept: application/json" https://pactols.frantiq.fr/opentheso/api/search?q=amphore&lang=fr&theso=TH_1
curl -L --header "Accept: application/ld+json"  https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1

curl -L --header "Accept: text/turtle"  https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1

Recherche par notation :
https://pactols.frantiq.fr/opentheso/api/search?q=notation:Guita1&theso=TH_1


On peut aussi obtenir les données dans un format spécifique en le précisant :
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=jsonld
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=json
curl  https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=turtle
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=rdf

on peut préciser la langue avec : &lang=fr
ou ne pas choisir de langue : On peut aussi obtenir les données dans un format spécifique en le précisant :
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=jsonld
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=json
curl  https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=turtle
curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&lang=fr&theso=TH_1&format=rdf

curl   https://pactols.frantiq.fr/opentheso/api/search?q=archi&theso=TH_1&format=rdf

on peut aussi filtrer par domaine/groupe/microthésaurus : &group=6
curl  https://pactols.frantiq.fr/opentheso/api/search?q=archi&theso=TH_1&lang=fr&group=6&format=rdf


Autocomplete
Permet de retourner les données sous forme de (id, valeur) en Json, ceci permet de faciliter la récupération des données pour des script d’indexation distant. 
Requête avec précision de la langue 
https://pactols.frantiq.fr/opentheso/api/autocomplete/arts?lang=fr&theso=TH_1
resultat = 
0	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtkOgxvd4Ijy"
label	"arts décoratifs"
1	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtGKMelLKwRd"
label	"arts mineurs"
2	
uri	"https://ark.mom.fr/Arkeo/26678/pcrt6YAjOsQDeM"
label	"arts textiles"
3	
uri	"https://ark.mom.fr/Arkeo/26678/pcrttq9gp2ZMuc"
label	"Arts"
4	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtcSQ6O32f6k"
label	"Artsakh"

Requête en incluant toutes les langues 
https://pactols.frantiq.fr/opentheso/api/autocomplete/arts?theso=TH_1
resultat = 
0	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtkOgxvd4Ijy"
label	"arts décoratifs"
1	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtGKMelLKwRd"
label	"arts mineurs"
2	
uri	"https://ark.mom.fr/Arkeo/26678/pcrt6YAjOsQDeM"
label	"arts textiles"
3	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtkOgxvd4Ijy"
label	"decorative arts"
4	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtGKMelLKwRd"
label	"minor arts"
5	
uri	"https://ark.mom.fr/Arkeo/26678/pcrt6YAjOsQDeM"
label	"textile arts"
6	
uri	"https://ark.mom.fr/Arkeo/26678/pcrttq9gp2ZMuc"
label	"Arts"
7	
uri	"https://ark.mom.fr/Arkeo/26678/pcrtcSQ6O32f6k"
label	"Artsakh"


Requête en précisant en plus le domaine ou microthésaurus ou groupe 
https://pactols.frantiq.fr/opentheso/api/autocomplete/arts?theso=TH_1&group=6
Le résultat est obtenu en filtrant les concepts qui appartiennent uniquement au domaine qui est donné en paramètre.


Recherche par Groupe ou Domaine / Microthésaurus …
On peut chercher un Groupe en précisant son Identifiant Ark :
https://pactols.frantiq.fr/opentheso/api/group/26678/pcrtnbDLi2FkAj
Toutes ces commandes sont possibles pour le header
curl -L --header "Accept: application/rdf+xml »
curl -L --header "Accept: text/turtle » 
curl -L --header "Accept: application/json »
curl -L --header "Accept: application/ld+json »

On peut chercher un Groupe en précisant son Identifiant interne :
https://pactols.frantiq.fr/opentheso/api/group/?id=5&theso=TH_1



Informations 
Pour connaître la dernière date de modification dans un thésaurus, on peut appeler l’URL suivante :
https://pactols.frantiq.fr/opentheso/api/info/lastupdate?theso=TH_1




Fonctions avancées

Comment retrouver une branche complète par autopostage en partant d’un concept vers le top terme (la racine) :
https://pactols.frantiq.fr/opentheso/api/expansion/concept?theso=TH_1&id=300&way=top

Comment retrouver une branche complète par autopostage en partant d’un concept vers le dernier terme spécifique (vers le bas) :
https://pactols.frantiq.fr/opentheso/api/expansion/concept?theso=TH_1&id=300&way=down


Requête en récupérer toute une branche d’un Groupe en particulier :
Ex : pour récupérer la branche complète du gorupe « 2 » du thésaurus « TH_1 » 
https://pactols.frantiq.fr/opentheso/api/all/group?id=2&theso=TH_1
en sépcifiant le format de données :
https://pactols.frantiq.fr/opentheso/api/all/group?id=2&theso=TH_1&format=rdf
https://pactols.frantiq.fr/opentheso/api/all/group?id=2&theso=TH_1&format=json
https://pactols.frantiq.fr/opentheso/api/all/group?id=2&theso=TH_1&format=turtle
https://pactols.frantiq.fr/opentheso/api/all/group?id=2&theso=TH_1&format=jsonld



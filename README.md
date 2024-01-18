# Pactols, un thésaurus pour l'archéologie
Le thésaurus Pactols est produit par la Fédération et Ressources sur l'Antiquité (<a href="http://www.frantiq.fr" target="_blank">Frantiq</a>, Réseau thématique du CNRS). Il est mis à disposition selon les termes de la licence <a [href="https://fr.wikipedia.org/wiki/Open_Database_License" target="_blank">ODC Open Database License (ODbL)</a> Les autorisations au-delà du champ de cette licence peuvent être obtenues à <a href="http://www.frantiq.fr" target="_blank">http://www.frantiq.fr</a>.

Pactols est l’unique vocabulaire français pour l’archéologie qui soit libre, multilingue (fr, en, de, it, es, nl, ar), normalisé (SKOS) et interopérable (ISO 25964). Il intègre pleinement les critères des principes FAIR, qui déterminent qu’une ressource propose des données Faciles à trouver, Accessibles, Interopérables et Réutilisables.
Élaboré à partir de la littérature scientifique recensée au <a href="http://catalogue.frantiq.fr" target="_blank">Catalogue collectif indexé</a> des bibliothèques du réseau Frantiq et des lexiques spécialisés, il est mis à jour avec l'aide des experts des domaines scientifiques et suit l'évolution de la discipline.
Pactols constitue un réservoir de métadonnées spécialisées utiles à l'indexation de toutes les ressources de la discipline : enregistrements de terrain, bases de données de travail et bibliographiques, publications et édition scientifique, valorisation du patrimoine archéologique, etc. Il couvre tous les sujets intéressant l'archéologie, depuis la Préhistoire jusqu'à laaa période actuelle, et les sciences de l'Antiquité.
Il tient son nom des branches hiérarchiques de sa version initiale : Peuples et cultures, Anthroponymes, Chronologie, Toponymes, Œuvres, Lieux, Sujets. Depuis septembre 2022, Pactols présente une nouvelle version 2 de 62.000 concepts, organisée en deux ensembles : 
-	les Lieux avec environ 50.000 concepts,
-	les Sujets avec 12.00 concepts. Les branches Sujets s’inspirent de la structure du BackBone Thesaurus développé par DARIAH Thesaurus Maintenance Working Group.

## Accès et réutilisation
Pactols est librement consultable ici: <a href="http://pactols.frantiq.fr" target="_blank">http://pactols.frantiq.fr</a> et ses données sont réutilisables (licence libre OdBL). 
- Depuis l’interface Opentheso et sans connexion particulière, chaque mot-clé peut être exporté dans les formats RDF/XML, Json, JsonLD et Turtle.
- Le thésaurus est aussi accessible via le Webservices REST de <a href="https://github.com/miledrousset/opentheso" target="_blank">Opentheso</a>.
- L’export de branches se fait à la demande, mais plusieurs exports sont à disposition dans ce dépôt.

## Organisation du dépôt
- Les fichiers d’export correspondent à des extractions des thésaurus en plusieurs formats. Ils sont mis à jour tous les 6 mois ou 1 an dans le dossier pactols_latest_version. 
Ils suivent l’organisation des collections thématiques de chacun des ensembles. Les versions anciennes sont archivées dans pactols_archives.
- Les listes recensent les nouveaux termes ajoutés (dossier pactols_candidats) et les concepts dépréciés (dossier pactols_deprecated). Ces derniers sont des concepts jugés obsolètes ou faisant doublon que l’on a retiré de la hiérarchie et qui ne sont pas/plus utilisables pour l’indexation. Ces listes sont mises à jour tous les 6 mois, en janvier et en juillet.
- La documentation utilisateurs est en cours de rédaction et sera déposée prochainement.


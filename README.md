Stage 4A STI INSA CVL
06 Juin 2017 - 04 Aout 2017

Stagiaire :  Juan PIRON
Entreprise : Telespazio France

Sujet du stage : etude de la gestion en configuration des demandes de flux PGL via le logiciel CAPIRCA.

Description : 
CAPIRCA est un logiciel développé par GOOGLE pour automatiser la création des ACL sur les firewalls.

Il prend en compte les access-list cisco et à ce titre devrait moyennant quelques adaptations, prendre en compte le firewall interne du CSG (PGL).

Le stagiaire étudiera la possibilité de migrer les règles existantes du PGL dans ce logiciel et mettra en place les mécanismes adéquat permettant la gestion de configuration des demandes flux.

 

Le stage consistera donc à

·         Adapter CAPIRCA pour la génération d’accès-list ASA (similaires à celles des routeurs cisco)

·         Mettre en place un mécanisme de génération des règles et de leur gestion en configuration (git ou subversion ?) à partir des demandes de flux utilisateurs.

·         Adapter les règles existante pour les injecter dans le système CAPIRCA.

Reformulation : 

1/ Créer un generator CiscoASA pour les routeurs PGL.

2/ 

a) Suffit de mettre capirca sur un remote repository de creer la policie ou de la modifer et de lancer le script python, suffit juste ensuite de faire git add, commit et push.
b) Mettre en place un remote repository sur GitHub permettant la gestion des différents ACLs (filters et policies (surtout)), tout cela directement dans les repertoires de pol et filters de capirca.

3/ créer les policies des ACLs déjà existante au niveau de PGLs


Compte-rendu journalier : 

06 Juin 2017 :
Visite rapide du CT + badge.
Prise en main de capirca.

07 Juin 2017 : 
Circuit arrivé. Revision de GitHub. Modif de aclgen.py pour le rep de dest des acls crées (filters).

08 Juin 2017 :
Debut de redaction du STB, et installation de Gobs sur une debian.

09 Juin 2017 :

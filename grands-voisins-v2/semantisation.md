
# Donnée sémantisée brute

C'est après le "direct mapping" avec:
```shell
 java -cp $JARS deductions.runtime.connectors.CSVImporterApp  "/home/jmv/data/Voisins sur site.csv" urn:gv/contacts/
```

```turtle
<urn:gv/contacts/row/6>
        a                              <http://vocab.sindice.net/csv/Row> ;
        <http://dbpedia.org/ontology/longName>
                "Amélie Thibierge" ;
        <http://vocab.sindice.net/csv/rowPosition>
                "6" ;
        <http://www.virtual-assembly.org/ontologies/1.0/pair#twitter>
                <https://twitter.com/apmediaorg> ;
        <http://xmlns.com/foaf/0.1/familyName>
                "Vo Trung" ;
        <http://xmlns.com/foaf/0.1/givenName>
                "Dung" ;
        <http://xmlns.com/foaf/0.1/homepage>
                <http://www.apmedia.org/site/> ;
        <http://xmlns.com/foaf/0.1/mbox>
                "dvotrung@icloud.com" ;
        <urn:gv/contacts/Activité>     "La société de presse \"Asie Pacifique Média\" édite \"AsiaPacNews\", un magazine en ligne consacré à l'Asie-Pacifique. De l'actualité aux analyses." ;
        <urn:gv/contacts/Arrivée>      "01/10/2016" ;
        <urn:gv/contacts/Bâtiment>     "CED" ;
        <urn:gv/contacts/Espace>       "Porte 8, 3ème étage" ;
        <urn:gv/contacts/Facebook>     <https://www.facebook.com/apmediaorg> ;
        <urn:gv/contacts/NomStructurePourAdministration>
                "La Ruche Denfert" ;
        <urn:gv/contacts/StructureJuridiqueSignatureConvention>
                "convention La Ruche" ;
        <urn:gv/contacts/Suivi>        "S'installe" ;
        <urn:gv/contacts/Thématiques>  "education et formation / Médias et numérique" ;
        <urn:gv/contacts/UrlLogo>      <http://www.apmedia.org/site/wp-content/uploads/2015/08/navi-logo.png> .
```

Colonnes après sémantisation brute:

- 'n° arrivee': <urn:gv/contacts/N°Arrivee>
- 'SUIVI': <urn:gv/contacts/Suivi>
- 'SITE WEB': <urn:gv/contacts/SiteWeb>		MEME_VALEUR_PARTOUT
- 'PRINT': <urn:gv/contacts/Print>		MEME_VALEUR_PARTOUT
- 'Nom structure pour administration': <urn:gv/contacts/NomStructurePourAdministration>
- 'Nom pour communication': <http://dbpedia.org/ontology/longName>
- 'Prénom interlocuteur référent': <http://xmlns.com/foaf/0.1/givenName>
- 'Nom interlocuteur référent': <http://xmlns.com/foaf/0.1/familyName>
- 'Slack': <urn:gv/contacts/Slack>
- 'Numéro contact': <http://xmlns.com/foaf/0.1/phone>
- 'Adresse e-mail': <http://xmlns.com/foaf/0.1/mbox>
- 'Prénom interlocuteur référent 2': <urn:gv/contacts/PrénomInterlocuteurRéférent2>
- 'Nom interlocuteur référent 2': <urn:gv/contacts/NomInterlocuteurRéférent2>
- 'Numéro contact 2': <urn:gv/contacts/NuméroContact2>
- 'Adresse e-mail 2': <urn:gv/contacts/AdresseE-mail2>
- 'Activité': <urn:gv/contacts/Activité>
- 'Site Web': <http://xmlns.com/foaf/0.1/homepage>
- 'Bâtiment': <urn:gv/contacts/Bâtiment>
- 'Espace': <urn:gv/contacts/Espace>
- 'Arrivée': <urn:gv/contacts/Arrivée>
- 'Contribution au projet proposée': <urn:gv/contacts/ContributionAuProjetProposée>
- 'Contribution réalisée': <urn:gv/contacts/ContributionRéalisée>
- 'Nombre salariés': <urn:gv/contacts/NombreSalariés>
- 'facebook': <urn:gv/contacts/Facebook>
- 'Compte twitter': <http://www.virtual-assembly.org/ontologies/1.0/pair#twitter>
- 'Linkedin': <urn:gv/contacts/Linkedin>
- 'NB de mentions presses': <urn:gv/contacts/NbDeMentionsPresses>	PAS_DE_DONNEES mais a garder !!!!!!!!!
- 'Ventes ou services': <urn:gv/contacts/VentesOuServices>	PAS_DE_DONNEES
- 'Structure juridique signature convention': <urn:gv/contacts/StructureJuridiqueSignatureConvention>
- 'Numéro de clé au PC': <urn:gv/contacts/NuméroDeCléAuPc>	PAS_DE_DONNEES mais a garder !!!!
- 'Propose du Bénévolat': <urn:gv/contacts/ProposeDuBénévolat>
- 'Projets au sein des GV': <urn:gv/contacts/ProjetsAuSeinDesGv>	PAS_DE_DONNEES  mais a garder !!!!
- 'URL logo': <urn:gv/contacts/UrlLogo>
- 'Assurance 2017': <urn:gv/contacts/Assurance2017>	PAS_DE_DONNEES : booléen !!!!!!!!!!!! admin
- 'N° contrat Link': <urn:gv/contacts/N°ContratLink>	PAS_DE_DONNEES
- 'Thématiques': <urn:gv/contacts/Thématiques>

## Champs ayant trait à la personne
- <http://xmlns.com/foaf/0.1/givenName>
- <http://xmlns.com/foaf/0.1/familyName>
- <http://xmlns.com/foaf/0.1/phone>
- <http://xmlns.com/foaf/0.1/mbox>
- <urn:gv/contacts/Slack>

### Champs hors formulaire de saisie
- <http://dbpedia.org/ontology/longName>
- <http://vocab.sindice.net/csv/rowPosition>
 
## Champs ayant trait à l'organisation et à sa gestion par GV
- <http://dbpedia.org/ontology/longName>
- <urn:gv/contacts/Facebook>
 - <urn:gv/contacts/Linkedin>
- <http://www.virtual-assembly.org/ontologies/1.0/pair#twitter>
- 
- <http://xmlns.com/foaf/0.1/homepage>
- <urn:gv/contacts/Activité>
- <urn:gv/contacts/Arrivée>   
- <urn:gv/contacts/Bâtiment>
- <urn:gv/contacts/Espace>
- 
- <urn:gv/contacts/ContributionAuProjetProposée>
- <urn:gv/contacts/ContributionRéalisée>
- 
- <urn:gv/contacts/ProposeDuBénévolat>
- <urn:gv/contacts/Thématiques>
- 
- <urn:gv/contacts/NomStructurePourAdministration>
- <urn:gv/contacts/NombreSalariés>
- <urn:gv/contacts/N°Arrivee>
- <urn:gv/contacts/Print>
- <urn:gv/contacts/SiteWeb>
- <urn:gv/contacts/StructureJuridiqueSignatureConvention>
- <urn:gv/contacts/Suivi> Enuméré:
	- <urn:gv/contacts/Suivi>
	- <urn:gv/contacts/Suivi> "Contacté" ;
	- <urn:gv/contacts/Suivi> "Contribue" ;
	- <urn:gv/contacts/Suivi> "En Cours" ;
	- <urn:gv/contacts/Suivi> "Parti" ;
	- <urn:gv/contacts/Suivi> "S'installe"
- <urn:gv/contacts/UrlLogo>

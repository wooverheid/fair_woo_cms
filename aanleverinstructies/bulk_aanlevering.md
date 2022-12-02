# How-to: bulk aanlevering Woo dossiers

## Lijst met dossiers
Bulk invoer gaat op basis van een `.csv` bestand met daarin per rij een dossier. 
In elke rij staan metadata van elk dossier. Hier is alleen de titel en een beschrijving verplicht. Echter hoe meer ingevuld wordt hoe rijker de publicatie pagina wordt, en ook hoe beter een zoekmachine over de dossiers zal werken. Alle gegevens die hier gevraagd worden staan in de brief met het besluit.

Naast de metadata bestaat een dossier uit een aantal bestanden. Die worden per rij weergegeven. **Zorg voor unieke bestandsnamen.** Per dossier kunnen 4 bestanden worden meegegeven: het besluit, het verzoek, de inventarislijst, en een zip bestand met daarin de losse vrijgegeven documenten.

De volgende kolommen dienen als eerste rij te bestaan:
| Titel | Type	| Beschrijving	| Thema	| Verzoekdatum	| Besluitdatum	| Beoordeling |	Verdaagd |	Verzoekdocument |	Besluitdocument	|
|----|----|----|----|----|----|----|----|----|----|

| Inventarisdocument|Bijlagen |	 	Verzoek |
|----|----|----|


- Titel: titel van het dossier (verplicht)
- Type: is het dossier een 'besluit op verzoek' of een 'actieve openbaarmaking'?
- Beschrijving: beschrijving van het dossier (verplicht)
- Thema: thema op basis van de ['Thema-indeling voor Officiële Publicaties (TOP-lijst)'](https://identifier.overheid.nl/tooi/set/scw_toplijst/1)
- Verzoekdatum/besluitdatum: datum van verzoek en besluit
- Beoordeling: keuze uit 'Openbaar', 'Deels openbaar', 'Reeds openbaar' of 'Niet openbaar'
- Verdaagd: 'Ja' als er sprake is van verdaging, 'Nee' als dit niet het geval was
- Verzoekdocument: bestandsnaam van het verzoekdocument (.pdf)
- Besluitdocument: bestandsnaam van het besluitdocument (.pdf)
- Inventarisdocument: bestandsnaam van een eventuele inventarislijst (.csv of .xlsx)
- Bijlagen: bestandsnaam van een zip met bijlagen (.zip)
- Verzoek: het uitgeschreven oorspronkelijke verzoek

Deze gegevens (op zijn minst een titel en beschrijving) dienen per dossier te worden ingevuld. 
Het document `dossier_template.csv` kan worden gebruikt als sjabloon voor het invullen van deze gegevens. Dit document bevat ook voorbeelden.

## Bestanden
Alle bestanden genoemd onder 'Verzoekdocument', 'Besluitdocument', 'Inventarisdocument' en 'Bijlagen' dienen in één map te worden geplaatst.

## Inventarisdocument
Elk dossier kan  worden voorzien van een inventarislijst.
Ook hier geldt: het is even werk, maar deze informatie is meestal bekend, en vaak (bijvoorbeeld via Zylab) al aanwezig. Het erbij leveren van deze inventaris helpt het zoeken naar de juiste documenten enorm.

De bestandsnamen in de eerste kolom komen overeen met de namen van de bestanden in de zip-file die is meegeleverd. 

De inventarislijst heeft  de volgende vorm (verwijs naar dit document onder de kolom 'Inventarisdocument' in de dossierlijst): (alleen de kolom bestandsnaam is verplicht)

| Bestandsnaam	| Titel |	Datum |	Documentsoort |	Beoordeling	| Uitzonderingsgrond	| Verzender | 	Ontvanger |	Beschrijving |
|---|---|---|---|---|---|---|---|---|

- Bestandsnaam: bestandsnaam van het document, dient aanwezig te zijn in een bijgevoegde zip met bijlagen (zie 'Lijst met dossiers') (verplicht)
- Titel: titel van het document
- Datum: datum van creatie/verzending van het document
- Documentsoort: het soort document, bijvoorbeeld 'Email' of 'Memo'
- Beoordeling: beoordeling van het individuele document, 'Openbaar', 'Deels openbaar', 'Reeds openbaar' of 'Niet openbaar'
- Uitzonderingsgrond: eventuele uitzonderingsgronden, gescheiden met een puntkomma `;`
- Verzender: verzender van het document
- Ontvanger: ontvanger van het document
- Beschrijving: beschrijving van het document

Het document `document_template.csv` kan worden gebruikt als sjabloon voor het invullen van deze gegevens. Dit document bevat ook voorbeelden.

Let er goed op dat de bestandsnaam overeen dient te komen met een bestand die is geplaatst in de zip met bijlagen bijbehorend aan het dossier!
Wanneer er een eigen gemaakte inventarislijst wordt toegevoegd worden enkel de documenten die in de lijst staan toegevoegd aan het dossier!

## Samenvattend

Als het goed is bestaan nu de volgende elementen:

* Een csv bestand met daarin een lijst van alle dossiers in het formaat beschreven onder 'Lijst met dossiers'
* Alle bestanden die zijn gelinkt aan een dossier (verzoek, besluit, inventaris of een zip met bijlagen) dienen in één enkele map te zijn geplaatst. Deze map mag in .zip aangeleverd worden.
*  De informatie per rij is precies hetzelfde als die per dossier wordt aangeleverd met het web-formulier. 



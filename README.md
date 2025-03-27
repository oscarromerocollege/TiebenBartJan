"# TiebenBartJan" 
Projectidee: Vliegtuig Database - "FlightFleet"
FlightFleet is een databaseapplicatie waarmee je informatie kunt beheren over verschillende vliegtuigen, inclusief hun specificaties, onderhoudshistorie, en status. Deze applicatie zal een CRUD-functionaliteit bieden om vliegtuigen toe te voegen, bij te werken, in te zien en te verwijderen, evenals extra functionaliteit voor het bijhouden van onderhoudsrecords en de status van de vliegtuigen.

1. Modellen en Relaties
Vliegtuig: Dit model bevat gegevens zoals vliegtuigtype, fabrikant, registratie, maximum capaciteit, snelheid, brandstofcapaciteit en vliegtuigstatus (actief, in onderhoud, buiten dienst).

Fabrikant: Informatie over de fabrikant van het vliegtuig, bijvoorbeeld Boeing, Airbus, enz.

Onderhoudsbeurt: Bevat gegevens over de onderhoudsbeurten van een vliegtuig, zoals datum van onderhoud, type onderhoud (routine, reparatie, enz.), en de monteur die het onderhoud heeft uitgevoerd.

Piloot: Gegevens over piloten die vliegtuigen besturen, inclusief hun naam, licentieniveau, en de vliegtuigen waarmee ze gecertificeerd zijn om te vliegen.

Relaties tussen modellen:
Vliegtuig - Fabrikant (Veel-op-1): Elk vliegtuig is geproduceerd door één fabrikant.

Vliegtuig - Onderhoudsbeurt (Een-op-veel): Elk vliegtuig kan meerdere onderhoudsbeurten hebben, maar een onderhoudsbeurt is voor slechts één vliegtuig.

Vliegtuig - Piloot (Veel-op-veel): Vliegtuigen kunnen door meerdere piloten worden bestuurd, en een piloot kan meerdere vliegtuigen besturen.

2. Gameplay Functies
CRUD-functionaliteiten:

Vliegtuigen: Gebruikers kunnen vliegtuigen toevoegen, bijwerken, inzien en verwijderen. Dit omvat het bijhouden van basisinformatie zoals vliegtuigtype, registratie, capaciteit en status.

Onderhoudsbeurten: Het beheren van onderhoudsbeurten voor elk vliegtuig. Dit kan een simpele lijst zijn van de afgelopen onderhoudsbeurten, inclusief details zoals de datum, type onderhoud, en kosten.

Fabrikanten: Beheer van vliegtuigfabrikanten en hun informatie, zoals naam en land van herkomst.

Piloten: Het toevoegen en bijwerken van piloten, inclusief hun kwalificaties en de vliegtuigen waarmee ze gecertificeerd zijn om te vliegen.

Zoekfunctionaliteit:

Gebruikers kunnen zoeken op vliegtuigtype, status, fabrikant, of onderhoudsgeschiedenis.

Je kunt filters toevoegen, bijvoorbeeld alleen vliegtuigen tonen die in onderhoud zijn of alle vliegtuigen van een specifieke fabrikant.

Beheer van onderhoud:

Het systeem houdt een gedetailleerd onderhoudsrecord bij voor elk vliegtuig. Elke keer dat er onderhoud wordt uitgevoerd, worden de details (datum, type onderhoud, kosten, enz.) geregistreerd.

Statusbeheer:

Het vliegtuig kan verschillende statussen hebben, zoals Actief, In Onderhoud, Buiten Dienst. Dit kan worden bijgehouden en geüpdatet via een dashboard.

3. Functionaliteiten en Structuur
Authenticatie en autorisatie:

Beheerders: Kunnen vliegtuigen, piloten, onderhoudsrecords en fabrikanten toevoegen of bewerken.

Gebruikers: Kunnen alleen de gegevens bekijken (afhankelijk van de autorisatie).

Eigen pagina’s:

Dashboard: Een overzichtspagina met een lijst van alle vliegtuigen, inclusief hun huidige status en sneltoetsen voor het toevoegen van nieuwe vliegtuigen of onderhoudsbeurten.

Vliegtuigdetails: Een gedetailleerde weergave van elk vliegtuig met de mogelijkheid om onderhoudsrecords, piloten en fabrikanten te beheren.

Onderhoudsoverzicht: Een pagina die een overzicht biedt van alle onderhoudsbeurten voor een specifiek vliegtuig, inclusief de datum en het type onderhoud.

Bootstrap: Je kunt Bootstrap gebruiken voor een nette en responsieve weergave van de vliegtuigen en onderhoudsrecords.

4. Technische Structuur en Onderdelen
Controllers: De controllers beheren de verschillende onderdelen van de database:

VliegtuigController: Beheer van vliegtuigen (CRUD).

FabrikantController: Beheer van vliegtuigfabrikanten.

OnderhoudController: Beheer van onderhoudsbeurten van vliegtuigen.

PilootController: Beheer van piloten en hun vliegtuigen.

Services: Deze logica wordt gebruikt voor het berekenen van bijvoorbeeld onderhoudskosten, het beheren van vliegtuigstatus, en het verwerken van gegevensinvoer.

Repositories: De repository-patronen worden gebruikt om gegevens op te slaan in de database, zoals vliegtuigen, fabrikanten, onderhoudsbeurten en piloten.

Viewmodels: Voor het beheren van de gegevens die naar de views worden gestuurd, zoals het formulier voor het toevoegen van vliegtuigen, onderhoudsbeurten en piloten.

Seeders: Om testdata in de database te laden, bijvoorbeeld om enkele vliegtuigen, fabrikanten en onderhoudsrecords te simuleren.

5. Mogelijke Uitbreidingen
Onderhoudskostenbeheer: Voeg functionaliteit toe om de kosten van elk onderhoudsbeurt bij te houden en een overzicht van de totale onderhoudskosten per vliegtuig te genereren.

Vliegtuighistorie: Voeg de mogelijkheid toe om de volledige geschiedenis van een vliegtuig in te zien, inclusief alle wijzigingen in status, onderhoudsbeurten en piloten die het hebben bestuurd.

Onderhoudsplanning: Voeg een functie toe waarmee beheerders onderhoud voor vliegtuigen kunnen plannen op basis van tijdsintervallen of vlieguren. Dit kan worden gebruikt om een onderhoudskalender te genereren.

Zoeken en filteren: Verbeter de zoekfunctionaliteit zodat gebruikers vliegtuigen kunnen zoeken op basis van meer geavanceerde criteria, zoals vliegtuigtype, fabrikant of onderhoudsstatus.

Notificaties: Voeg een notificatiesysteem toe dat de beheerder waarschuwt wanneer een vliegtuig onderhoud nodig heeft of wanneer een onderhoudsbeurt is uitgevoerd.

Samenvatting
Het FlightFleet-project biedt een uitgebreid vliegtuigbeheersysteem waarin je vliegtuigen, onderhoudsbeurten, piloten en fabrikanten kunt beheren. Het biedt een gebruiksvriendelijke interface voor het beheren van gegevens, het bijhouden van vliegtuigstatus en onderhoud, en het plannen van toekomstige onderhoudsbeurten. Door gebruik te maken van ASP.NET MVC kun je het project goed structureren en uitbreiden naar de gewenste functionaliteit.

Dit idee combineert de noodzaak voor een databasebeheerder met een specifieke toepassing in de luchtvaartindustrie, wat een unieke en interessante uitdaging vormt voor je eindwerk!

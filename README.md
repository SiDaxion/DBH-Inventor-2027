# DBH Inventor 2027

**Schooleigen CAD-omgeving voor Autodesk Inventor 2027**  
Don Bosco Hoboken | Afdeling Mechanica en Lassen

DBH Inventor 2027 is ontwikkeld om Autodesk Inventor 2027 volgens de CAD-standaarden van de school in te richten. Het project voorziet in schooleigen sjablonen, materialen, projectinstellingen, persoonlijke CAD-opslag en een grafisch startprogramma met controles, herstel en automatische updates.

DBH Inventor 2027 is een **afzonderlijke productlijn** naast andere versies van DBH Inventor. Het is geen upgrade of vervanging van een andere DBH Inventor-installatie.

> **Let op:** DBH Inventor 2027 installeert Autodesk Inventor zelf niet en verstrekt geen Autodesk-licentie. Autodesk Inventor 2027 moet vooraf correct geïnstalleerd en gelicentieerd zijn.

> **Beschikbaarheid:** De 2027-toepassing bevindt zich nog in de testfase. Er is nog geen publieke installatierelease vrijgegeven. Gebruik uitsluitend een installatiebestand dat na validatie via de [officiële GitHub Releases](https://github.com/SiDaxion/DBH-Inventor-2027/releases) wordt aangeboden.

## Wat bevat DBH Inventor 2027?

- Schooleigen, voor Inventor 2027 aangeleverde sjablonen voor onderdelen, plaatwerk, samenstellingen, lasconstructies, tekeningen en presentaties.
- Bijbehorende **Design Data**, materialenbibliotheek en Application Options.
- Een eigen Inventor-project voor 2027, met een persoonlijke **Werkmap** en **ContentCenter**.
- Een grafisch startprogramma op basis van .NET 10, met interne PowerShell-onderdelen voor beheer en opstart.
- Controle, veilig archiveren en herstel van beheerde schoolbestanden, gescheiden van persoonlijke CAD-werkbestanden.
- Een afzonderlijke installatie-identiteit, snelkoppeling en voorzien updatekanaal voor Inventor 2027.

De compatibiliteit van de overgenomen Design Data, materialen en Application Options met Autodesk Inventor 2027 moet nog in de praktijk worden bevestigd.

## Vereisten

- Een Windows-computer met een geschikte 64-bits omgeving.
- **Autodesk Inventor 2027**, vooraf geïnstalleerd en correct gelicentieerd.
- Een toegankelijk persoonlijk Windows-gebruikersprofiel, met opslagruimte voor de Werkmap en ContentCenter.
- Internettoegang voor het downloaden van vrijgegeven installatiebestanden en toekomstige updates.

De software is ontworpen voor installatie **per Windows-gebruiker**, zonder standaard beheerdersrechten voor de eigen gebruikersinstallatie. De daadwerkelijke werking en installatie op beheerde schoolcomputers moeten nog getest worden. Het ICT-beleid kan aanvullende toestemming vereisen.

## Installeren

Zodra een geteste installatieversie is vrijgegeven:

1. Open de [GitHub Releases](https://github.com/SiDaxion/DBH-Inventor-2027/releases).
2. Kies de nieuwste **stabiele release voor DBH Inventor 2027** en download het bijbehorende installatiebestand onder **Assets**.
3. Sluit Autodesk Inventor volledig af voordat je de installatie uitvoert.
4. Start het installatiebestand en volg de instructies.
5. Gebruik daarna de eigen bureaubladsnelkoppeling **Inventor 2027 - DBH Mechanica**.

Gebruik uitsluitend een installatiepakket dat expliciet bedoeld is voor DBH Inventor 2027. Volg op centraal beheerde computers de instructies van school-ICT.

## Starten, controleren en bijwerken

De grafische launcher is ontworpen rond vier stappen:

**Controleren → Updates → Voorbereiden → Inventor starten**

Bij het starten controleert DBH de beheerde schoolbestanden. Ontbrekende of gewijzigde bestanden kunnen worden hersteld vanuit een gecontroleerde installatiebron. Afwijkende schoolbestanden worden waar nodig eerst veilig gearchiveerd. **Persoonlijke CAD-werkbestanden worden niet als beheerde installatiebestanden behandeld.**

De updatefunctionaliteit is bedoeld om uitsluitend goedgekeurde **stabiele releases van DBH Inventor 2027** te gebruiken. De bestaande beveiligingscontroles omvatten onder meer productjaar, versie, bestandsgrootte en SHA-256. Automatisch downgraden of overschakelen naar een release van een andere DBH Inventor-versie is niet de bedoeling.

Het afzonderlijke GitHub-updatekanaal moet vóór de eerste publieke 2027-release correct worden ingesteld en daadwerkelijk getest. Zolang geen release beschikbaar is, kan er ook geen 2027-update worden geïnstalleerd.

## Persoonlijke Werkmap en ContentCenter

Persoonlijke CAD-bestanden blijven gescheiden van de beheerde installatie. Bij een eerste inrichting krijgt een geschikte **school-OneDrive** de voorkeur. Als die niet beschikbaar is, wordt de persoonlijke Windows-map **Documenten** gebruikt.

Een bestaande opslaglocatie wordt niet stilzwijgend gewijzigd. Als de school-OneDrive later beschikbaar komt, is een gecontroleerd migratievoorstel voorzien met de keuzes **Migreren** en **Nu niet**. Persoonlijke bestanden mogen daarbij niet automatisch worden overschreven of verwijderd.

De persoonlijke opslag is als volgt ingericht:

```text
DBH_Inventor_2027/
├── Werkmap/
│   ├── Onderdelen/
│   ├── Samenstellingen/
│   ├── Tekeningen/
│   └── Presentaties/
└── ContentCenter/
```

De werkelijke locatie wordt bepaald door Windows en de persoonlijke DBH-configuratie. **Verplaats of verwijder deze mappen niet zonder back-up en controle.**

De beheerde programmabestanden, technische beheeronderdelen en het onafhankelijke archief hebben eigen 2027-mappen onder `%LOCALAPPDATA%`. De gegevens van DBH Inventor 2027 en andere DBH Inventor-versies zijn ontworpen om gescheiden te blijven.

## Samen met een andere versie van DBH Inventor

DBH Inventor 2027 is ontworpen om **afzonderlijk naast andere versies van DBH Inventor geïnstalleerd** te kunnen worden, zonder elkaars bestanden te wijzigen. Iedere productlijn heeft een eigen installatie-identiteit, projectbestand, snelkoppeling, Werkmap, ContentCenter, archief en updatebron.

Deze scheiding moet bij gebruik naast een andere DBH Inventor-versie nog met echte Windows-installatie-, opstart- en verwijdertests worden bevestigd. **Gelijktijdig uitvoeren** van verschillende Inventor-jaargangen is niet gegarandeerd en moet afzonderlijk worden onderzocht.

## Schooluitrol en ICT

De eerste 2027-uitgave is bedoeld voor lokale validatie voordat er een bredere schooluitrol plaatsvindt. Daarbij moeten onder andere gebruikersrechten, projectactivatie, sjablonen, Design Data, materialen, persoonlijke opslag, beveiligingscontroles en de scheiding ten opzichte van andere DBH Inventor-versies worden getest.

Er is **nog geen afzonderlijke schoolbootstrap voor DBH Inventor 2027** beschikbaar. Een bootstrap die voor een andere DBH Inventor-versie is ontwikkeld, mag niet zonder afzonderlijke validatie voor de 2027-productlijn worden gebruikt.

Schakel Windows-beveiliging of Microsoft Defender SmartScreen niet uit om een installatie te forceren. Gebruik uitsluitend gecontroleerde installatiebestanden uit de officiële repository.

## Verwijderen

Wanneer de 2027-software is geïnstalleerd, wordt ze afzonderlijk verwijderd via **Windows-instellingen → Apps → Geïnstalleerde apps**.

De verwijderprocedure is ontworpen om de beheerde 2027-installatieonderdelen op te ruimen, met behoud van persoonlijke **Werkmap**, **ContentCenter** en het onafhankelijke 2027-archief. Autodesk Inventor 2027 zelf en installaties van andere DBH Inventor-versies mogen niet worden verwijderd of gewijzigd. Deze bescherming moet bij de eerste installatietests nog praktisch worden bevestigd.

## Ondersteuning en releases

- [Releases en downloadbestanden](https://github.com/SiDaxion/DBH-Inventor-2027/releases)
- [Problemen melden of verbeteringen voorstellen](https://github.com/SiDaxion/DBH-Inventor-2027/issues)

De **releaseopmerkingen** beschrijven per vrijgegeven versie de nieuwe functies, verbeteringen, opgeloste problemen en eventuele installatieaandachtspunten. Deze README beschrijft het product en de algemene werking en wordt alleen aangepast bij structurele wijzigingen.

Vermeld bij een probleem de gebruikte DBH-versie, de uitgevoerde handeling en de exacte foutmelding. Deel geen wachtwoorden, persoonsgegevens of vertrouwelijke leerlingbestanden in openbare GitHub Issues.

---

*DBH Inventor 2027 is een schooleigen CAD-configuratie voor Autodesk Inventor 2027. Het is geen officieel Autodesk-product en bevat geen Autodesk-softwarelicentie.*

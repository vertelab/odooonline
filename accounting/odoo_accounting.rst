.. _odooaccounting:

==========================
Bokföring i Odoo
==========================


Den här sidan sammanfattar hur Odoo behandlar typiska konton och transaktioner.

Dubbelbokföring
------------------------
Odoo skapar automatiskt alla verifikat bakom kulisserna för var och en av dina bokföringstransaktioner: kundfakturor, försäljningsorder, utgifter, lagerförflyttningar etc.

Verifikaten skapas på traditionellt sätt med regler för dubbel bokföring och använder i normala fall BAS-kontoplanen.

Periodiseringsmetoder och kassakrav
------------------------------
Odoo stöder både periodiserad och kontantbaserad rapportering. Detta gör att du kan redovisa intäkter / kostnader när transaktioner inträffar (dvs periodiseringsbas) eller när betalning görs eller erhålls (dvs. kontantbas).

Multi-företag
---------------
Odoo tillåter att hantera flera företag inom samma databas. Varje företag har sin egen kontoplan och regler. Du kan få konsolideringsrapporter enligt dina konsolideringsregler.

Användare kan komma åt flera företag men arbetar alltid i ett företag i taget.

Multi-valutor
----------------
Varje transaktion registreras i företagets standardvaluta. För transaktioner som sker i en annan valuta lagrar Odoo både värdet i företagets valuta och värdet i transaktionsvaluta. Odoo kan generera valutor vinster och förluster efter avstämning av journalposter.

Valutakurserna uppdateras en gång om dagen med en yahoo.com webbtjänst.


Kundfordringar och betalningsbara
-----------------------------
Som standard använder Odoo ett enda konto för alla kontofordringar och en för alla betalningsuppgifter. Du kan skapa separata konton per kund / leverantör, men du behöver inte.

Eftersom transaktioner är knutna till kunder eller leverantörer får du rapporter för att utföra analys per kund / leverantör, såsom kundredovisning, intäkter per kund, åldersfordringar / skulder, ...

Brett utbud av finansiella rapporter
-------------------------------
I Odoo kan du generera finansiella rapporter i realtid. Odoos rapporter sträcker sig från grundläggande redovisningsrapporter till avancerade hanteringsrapporter. Odoo rapporter inkluderar:

* Prestationsrapporter (som vinst och förlust, budgetvariation)
* Placeringsrapporter (t.ex. Balansräkning, Åldersbetalning, Åldersfordringar)
* Kontantrapporter (som banköversikt)
* Detaljrapporter (t.ex. försöksbalans och huvudbok)
* Hanteringsrapporter (t.ex. budgetar, sammandrag)
* Odoos rapportmotor gör att du kan anpassa din egen rapport utifrån dina egna formler.

Importera bankfeeds automatiskt
-------------------------------
Bankavstämning är en process som matchar dina bankkreditslinjer, enligt bankens uppgifter, till dina bokföringstransaktioner i huvudboken. Odoo gör bankavstämningen lätt genom att importera kontoutdrag från din bank direkt till ditt Odoo-konto. T ex Bankgirot, SEB eller Swedbank. Det innebär att du kan få en daglig översikt över ditt kassaflöde.

Odoo påskyndar bankavstämningen genom att matcha de flesta av dina importerade transaktionsrader till dina bokföringstransaktioner. Odoo kommer också ihåg hur du har behandlat andra transaktioner och tillhandahåller förslag till bokföring.

Beräknar den skatt du är skyldig till din skattemyndighet
---------------------------------------------
Odoo uppräknar alla dina bokföringstransaktioner för din skatteperiod och använder dessa summor för att beräkna din skattskyldighet. Du kan då kolla din moms genom att köra Odoos Skatterapport.

Inventarvärdering
-------------------
Odoo stöder både periodiska (manuella) och eviga (automatiska) inventeringsvärderingar. De tillgängliga metoderna är standardpris, genomsnittspris, LIFO (för länder som tillåter det) och FIFO.

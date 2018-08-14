.. _kreditfaktura:

.. index::
   single: Create credit note from sales order


Kreditfaktura (fakturan är helt fel)
-------------------------------
En felaktig faktura har skapats i Odoo, den behöver elimineras. Använd knappen "kreditfaktura" och välj alternativet: Avbryt: skapa kredit och stäm av. Då kommer Odoo att skapa en ny kreditfaktura som eliminerar den aktuella fakturan. Sedan sker en avstämning mellan de två fakturorna så att de märks "betald". Bokföringsmässigt så skapas två motstående verifikat som nollar ut transaktionen. 

Har kunden redan fått den felaktiga fakturan, skicka då kreditfakturan och informera att de inte skall betala den ursprungliga fakturan. 
Har kunden däremot redan betalat fakturan måste även betalningen nollas och beloppet återbetalas. Detta sker så här:....
   
   accounting/refund_invoice.rst


Kreditfaktura (fakturan skall rättas)
-------------------------------
En felaktig faktura har skapats i Odoo, den behöver ändras. Använd knappen "kreditfaktura" och välj alternativet: Ändra: skapa kredit och stäm av och skapa en ny faktura i utkast. Då kommer Odoo att skapa en ny kreditfaktura som eliminerar den aktuella fakturan. Sedan sker en avstämning mellan de två fakturorna så att de märks "betald". Bokföringsmässigt så skapas två motstående verifikat som nollar ut transaktionen. En ny faktura skapas som en kopia av den ursprungliga fakturan. Denna är redigeringsbar och kan korrigeras-

Har kunden redan fått den felaktiga fakturan, skicka då kreditfakturan och informera att de inte skall betala den ursprungliga fakturan utan den nya.

Korrigera mindre fel
-------------------------------
En felaktig faktura har skapats i Odoo, du kommer överens om att korrigera felaktigheten på nästa faktura. I detta fall behövs inte någon kredirfaktua. På nästa faktura som skapas till kunden kan extra rader läggas in som korrigerar t ex ett förhögt belopp på en ridigare faktura.

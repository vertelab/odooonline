
======================================
Försäljning av varor från Sverige till en plats utanför EU (export, SKV 560, exempel 14) 
======================================

.. image:: skv560/exempel14.jpg 
   :align: center

Bilhandlaren Sonja i Sverige säljer en begagnad bil till privat-
personen Salomon i Schweiz för 100 000 kr. Salomon
hämtar bilen hos Sonja i Sverige och kör den själv till
Schweiz.

Eftersom Sonja levererar bilen i Sverige måste hon
deklarera och betala moms i Sverige. Hon kan i efterhand
betrakta försäljningen som exportomsättning och återbetala
momsen till Salomon. Ett villkor för detta är att hon fått
handlingar som styrker att bilen förts ut ur EU och att
den har avregistrerats i vägtrafikregistret. (TODO)

Odoo väljer automatiskt skatteregionen "Handel med världen" eftersom Salomon har en adress i Schweiz. Om kunen 
har en adress inom EU eller en adress i Sverige så sker matchningen med respektive skatteområde. Fakturan märks med texten Export.

Regionsmatchningen sker i följande steg

1. Matcha land, stat och postkod som är angivet på kundkortet.
2. Matcha land och stat.
3. Matcha land.
4. Matcha landsgrupp.
5. Matcha mot en skatteregion som ej har något av ovanstående krav.

Om Nore av något skäl skulle skatta enligt någon annan modell kan detta beteende överridas genom att ange korrekt skatteområde på kundkortet (rätt skatteområde väljs automnatiskt varje gång) eller specifikt på inköpsorder eller leverantörsfaktura (rätt skatteområde för en enskild transaktion).


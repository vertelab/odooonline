.. _skv560_example_1:

.. index::
   single: Försäljning av varor till ett annat EU-land

======================================
Försäljning av varor till ett annat EU-land (SKV 560, exempel 1) 
======================================

.. image:: skv560/exempel1.jpg 
   :align: center

Svea i Sverige säljer en maskin till Bastien i Belgien för
100 000 kr. Båda är beskattningsbara personer och är
momsregistrerade i respektive hemland. Maskinen
transporteras från Sverige till Belgien.
Sveas omsättning i Sverige är undantagen från skatte-
plikt här. Bastien i Belgien gör ett unionsinternt förvärv.

Odoo väljer automatiskt skatteregionen "Handel med världen" eftersom Bastien har ett skatteregistreringsnummer och en adress i Belgien. Om kunden 
har en adress inom EU eller en adress i Sverige så sker matchningen med respektive skatteområde. Fakturan märks med texten Export.

Regionsmatchningen sker i följande steg

1. Matcha land, stat och postkod som är angivet på kundkortet.
2. Matcha land och stat.
3. Matcha land.
4. Matcha landsgrupp.
5. Matcha mot en skatteregion som ej har något av ovanstående krav.

Om Bastien av något skäl skulle skatta enligt någon annan modell kan detta beteende överridas genom att ange korrekt skatteområde på kundkortet (rätt skatteområde väljs automatiskt varje gång) eller specifikt på inköpsorder eller leverantörsfaktura (rätt skatteområde för en enskild transaktion).


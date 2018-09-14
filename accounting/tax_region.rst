.. _tax_region:

.. index::
   single: Skatteområde

======================================
Skatteområde
======================================
Ett skatteområde beskriver skillnader i hur skatter hanteras beroende på var kunden/leverantören befinner sig. De normala bokföringsinställningarna på produkter är att konton och skatter gäller vid handel inom Sverige. När man skapar en säljorder, inköpsorder, faktura, etc så kan man välja att knyta den till ett visst skatteområde. Konton och skatter på produkterna kommer då översättas till de konton och skatter som ska användas för handel med det specifika skatteområdet.

Automatiskt skatteområde
-----------------------
När man skapar ett dokument som kan ha ett skatteområde (t.ex. en faktura) så försöker Odoo automatiskt identifiera korrekt skatteområde utifrån kundens **land** och **skatteregistreringsnummer** (VAT). Alternativt så kan man på kundkortet direkt fylla i vilket skatteområde som ska användas. Detta sker i följande steg, där det första skatteområdet som matchar kommer att användas.

1. Välj den skatteregion som specificerats på kundkortet.
2. Om säljaren har ett VAT-nummer, regionsmatcha mot skatteregioner som kräver VAT.
3. Regionsmatcha mot skatteregioner som ej kräver VAT.

Regionsmatchning
================

1. Matcha land, stat och postkod.
2. Matcha land och stat.
3. Matcha kundens land mot skatteområdets land.
4. Matcha kundens land mot skatteområdets landsgrupp.
5. Matcha mot en skatteregion som ej har något av ovanstående krav.

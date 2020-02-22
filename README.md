# Project_2

## Key Questions

1. Did increasing avocado prices cause avocado imports to increase and imports of other crops to decrease (Kaggle and USDA)?
2. As prices went up how did domestic and import amount change (USDA)?
3. Does the time of year affect the price of avocados?
4. Does the pric of avocados affect the stock price of Chipotle?

## Data sources

We used an avocado price data set from Kaggle (CSV), Yahoo Finance API for Chipotle stock price, and United States Department of Agriculture Foreign Agricultural Service data (CSV)

## Summary

1. We did not see any obvious change to the production of other crops as avocados ramped up.

<img src="Images/avo_corn.png" width="60%">
<img src="Images/avo_mango.png" width="60%">
<img src="Images/avo_lime.png" width="60%">

2. Yet to be determined import/dometic production relation.
3. There was a dip in avocado prices near the beginning of the year for four of the five years considered.
4. There was a significant drop to Chipotle stock in one case where avocado prices shot up.

<img src="Images/cmg_and_avo_prices.png" width="60%">

## ETL Steps

1. FSDA data was in a two way table. Used iloc to change to one way.
2. Yahoo finance API gave daily stock close values, but the Kaggle data was weekly (Sunday). The last day of the weeks close for Chipotle was used for price on Sunday.

## SQL tables

- avocado_price
- avocado_imports
- corn_imports (herman)
- lime_imports (terri)
- mangos_imports (nick)
- sorghum_imports (molly)
- strawberries
- peaches

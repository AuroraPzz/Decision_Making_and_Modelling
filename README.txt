------------------------------------------------------------------------------------------------------------------------------------
# Project
------------------------------------------------------------------------------------------------------------------------------------

File POSdata.csv reports the data on products A, B, C, D sales in 46 different 24/365 point of sales (POS) 
between October 2036 and November 2037.

## Each record has the following seven fields:

 - DateTime: purchase time (YYYY-MM-DD-hh.mm.ss, e.g., 2038-12-01-02.31.05 means that someone 
   purchased some products on December 2038, 1st at 2:31:05);

 - PointOfSale: point of sale unique identifier;

 - Error: error-detecting code. If it is equal to 1, 
   incorrect data has been recorded and the record should be disregarded;

 - ProductA: number of products A sold;

 - ProductB: number of products B sold;

 - ProductC: number of products C sold;

 - ProductD: number of products D sold.

***

Products A, B, C, D are perishable the products unsold at midnight must be disposed.

Each POS must reorder the products each day at 18:00 and they become available at the POS a 00:00:01 
of the next day. As an example, if a POS orders 20 products A on August 2036, 20th, it will receive the 
20 products on August 2036, 21st at 00.00.01.

Each POS sells products A, B, C, D for 50.00, 20.00, 100.00, 10.00 euro per unit respectively and 
purchase them from its supplier for 37.00, 15.00, 70.00, 8.00 euro respectively.

The supplier pays 30.00, 10.00, 50.00, 7.00 euro to make a unit of product A, B, C, D respectively.

***

1. Use the data recorded between October 2036 and July 2037 for the first 30 POSs to develop a 
   method to apply to all the 46 POSs to forecast their sales day-by-day between August 2036 and 
   November 2037. As an example, each POS should use your method on August 2026, 20th to forecast 
   its sales of August 2026, 21st. The different POSs can share their data. Determine the profits of each 
   POS and of its supplier between August 2036 and November 2037. Report and comment both the 
   overall profits of the period and the day-by-day profits. Employ your forecasting method also to 
   answer to the following points.

2. Each POS can use the data of all the 46 POSs recorded between October 2036 and July 2037 to 
   negotiate the product purchase prices with its supplier. Determine if new purchase prices can be 
   defined so that both the POS and supplier profits can increase; compute the POS and the supplier 
   profits between August 2036 and November 2037; compare these profits with the ones computed at 
   Point 1.

3. POSs can consort and negotiate as a single actor new purchase prices with the supplier based on the 
   data of all the 46 POSs recorded between October 2036 and July 2037. Determine if new purchase 
   prices can be defined so that both the overall profits of the POSs and the supplier profit can increase; 
   compute the overall profits of the POSs and the supplier profit between August 2036 and November 
   2037; compare these profits with the ones computed at Points 1 and 2.

4. The application of the new purchasing prices determined at Point 3 may induce fewer profits than the 
   ones obtained at Point 2 for some POSs. Using the data recorded between October 2036 and July 
   2037 forecast which POSs could be affected by this kind of loss. Define and justify a policy that allows 
   POSs to transfer part of the profits to other POSs so that no one of them suffer loss of profit.

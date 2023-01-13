# Bean Drop Overview
This file has been created to help understand the various Bean Drop Projects and how they work together and integrate into the 'Bean Drop Process Cycle'.

## Chapters:
1. Bean Drop Concept Overview
2. Project Overviews
    - Bean Drop Point of Sale device
    - Bean Drop Station
    - Bean Drop Processing Center
    - Bean Drop Django website
    - Bean Drop Station NB_IOT_module
    - Bean Drop Station micro-controller
    
# Bean Drop Concept Overview
Bean Drop is a newly proposed service to replace single-use coffee cups in cafes by introducing a reusable cup collection, cleaning and redistribution service.
Takeaway drinks in cafes are served to customers in Bean Drops reusable cups; customers enjoy their drink as normal and then return the cup to a Bean Drop Station instead of a recycling bin; this allows the cups to be collected, cleaned and redistributed to cafes by Bean Drop. 
This circular economy of reusing cups reduces the carbon footprint of takeaway drinks.

![Bean Drop Cycle - Email](https://user-images.githubusercontent.com/57590322/206234124-574db8af-0759-47d2-b0f0-8db0b5ef9525.png)

Bean Drop Resuable Cups contain a small electronic tag in the bottom of the cup; allowing cups to traced. 
Cups will be scanned during all steps of the process cycle, between Bean Drop, Businesses and Customers.

Businesses scan Bean Drop Reusable cups using provided Point of Sale devices and serve/sell drinks in them to customers. The transaction is registered on a global database.

Tracing cups allows cups to be linked to customer accounts.
Customer accounts are tracked on a global database. Bean Drop will charge an initial cup deposit to customers on their first purchase, by returning a cup to a Bean Drop Station;
their customer account is updated and the deposit is placed back into their account. The customer may then take out a new clean Bean Drop resuable cup without any additional charge; 
the deposit is transfered to the new cup, and so on and so on. Customers may request the deposit refunded back to at anypoint as long as they have returned their cups to the Bean Drop Stations.

## Project Overviews
### [Bean Drop Point of Sale device](https://github.com/henryjwillson/bean_drop_point_of_sale)
The Bean Dop Point of Sale device is a device provided to businesses/cafes to allow scanning and linking of bean drop resuable cups to the global database during transactions with customers.
Scanning cups at the point of sale device links each cup to a customer.

### [Bean Drop Station](https://github.com/henryjwillson/bean_drop_station)
The Bean Drop Station is a 'smart bin' which identifies cups when customers return them. Customers place their cups in the Bean Drop Station, and with a combination of sensors;
 it is able to identify the cup and update the customer account on the global database. This allows customers to get a new cup at their nearest cafe without any additional deposit charge.

### [Bean Drop Processing Center](https://github.com/henryjwillson/bean_drop_processing_centre)
Software user interface designed to allow Bean Drop employees to conduct daily tasks easily and quickly whilst interacting with the global database. Examples include; 
delivering a crate of resuable cups to a cafe, thus the updating of the database to register that transaction. 
Collecting cups from a Bean Drop Station is another example where the database is required to be updated to understand which Bean Drop Stations need emptying / collecting again to prevent overflow.

### [Bean Drop Django Website](https://github.com/henryjwillson/bean_drop_django_website)
A website built on the Django framework as a location for customers to access and manage their Bean Drop accounts and a place for Bean Drop to advertise certain features and it's service to other companies.

### Bean Drop Station NB_IOT_module
Communication module within the Bean Drop Station, allowing it to communicate with Bean Drop servers and update the global database.

### Bean Drop Station micro-controller
Internal micro controller used to control numerous sensors and motors within the Bean Drop Station.
